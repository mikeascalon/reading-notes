# Reading Notes

## Django Custom User

### What are the key benefits of using a Django Custom User Model, and how does it differ from the default Django User Model?

While the default Django User Model is sufficient for many projects, the flexibility, customization, and future-proofing offered by a custom user model make it a beneficial choice for projects with specific or evolving user management requirements. Starting a Django project with a custom user model is generally recommended to avoid the difficulties associated with changing the user model mid-project.

Explain the process of creating and implementing a Custom User Model in Django, including the necessary changes to settings.py and the required model fields.

1. Start a New Django Project and App
   
2. Define the Custom User Model

* In your app (e.g., app), create a model that extends `AbstractBaseUser` and, optionally, `PermissionsMixin` to handle permissions. This gives you the flexibility to define your own fields and methods. Here's a basic example:

```python
from django.contrib.auth.models import AbstractBaseUser, BaseUserManager, PermissionsMixin
from django.db import models

class MyUserManager(BaseUserManager):
    def create_user(self, email, password=None, **extra_fields):
        if not email:
            raise ValueError('The Email field must be set')
        email = self.normalize_email(email)
        user = self.model(email=email, **extra_fields)
        user.set_password(password)
        user.save(using=self._db)
        return user

    def create_superuser(self, email, password=None, **extra_fields):
        extra_fields.setdefault('is_staff', True)
        extra_fields.setdefault('is_superuser', True)

        if extra_fields.get('is_staff') is not True:
            raise ValueError('Superuser must have is_staff=True.')
        if extra_fields.get('is_superuser') is not True:
            raise ValueError('Superuser must have is_superuser=True.')

        return self.create_user(email, password, **extra_fields)

class MyUser(AbstractBaseUser, PermissionsMixin):
    email = models.EmailField(unique=True)
    is_active = models.BooleanField(default=True)
    is_staff = models.BooleanField(default=False)
    # Add additional fields here

    objects = MyUserManager()

    USERNAME_FIELD = 'email'
    REQUIRED_FIELDS = []  # Email & Password are required by default.

```
  
3. Update settings.py

In your Django project's `settings.py`, specify your custom user model with the `AUTH_USER_MODEL` setting. This tells Django to use your custom model instead of the default user model.

```python
AUTH_USER_MODEL = 'myapp.MyUser'

```

4. Create and Apply Migrations

```python
python manage.py makemigrations myapp
python manage.py migrate

```
5. Use the Custom User Model

Now, your Django project is configured to use the custom user model. Whenever you reference the user model in your project, you should use Django’s get_user_model method instead of directly referring to the model. This ensures compatibility across your project.

```python
from django.contrib.auth import get_user_model

User = get_user_model()

```

6. Creating Superuser

To create a superuser account, use the createsuperuser command. You'll be prompted to enter the email and password for the superuser, according to the custom user model definition.

## What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project.

DjangoX is a framework built on top of Django, designed to provide developers with a more extended and ready-to-use project template that includes a set of additional tools, configurations, and third-party packages pre-integrated to speed up the development process. It's not an official extension of Django but rather a community-driven project aimed at enhancing the Django development experience by including features that are commonly required for web applications but not provided by Django out of the box.

Imagine you're starting a new web project that requires a  user management system, social authentication, and needs to be deployed quickly for user testing. Instead of spending time configuring these features from scratch, you can use DjangoX as your project base.

### Resoucres

[Django Custom User Model](https://learndjango.com/tutorials/django-custom-user-model)

[DjangoX](https://github.com/wsvincent/djangox)

[ChatGPT](https://chat.openai.com/)