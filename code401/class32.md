# Reading Notes

## DRF Permissions, generic view and SQL review

What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?

**Permission Classes:** DRF provides a set of permission classes that determine whether a request should be granted or denied access. These classes include permissions for read-only access, authentication required, custom permissions, etc.

**Authentication Classes:** While not permissions themselves, authentication classes work closely with permissions to identify the user making a request. Permissions can then use this information to make access decisions.

**Object-Level Permissions:** In addition to global permissions that apply to all instances of a model, DRF supports object-level permissions. This allows permissions to be applied to individual objects, enabling fine-grained access control.

**Throttling:** Throttling limits the rate of requests a user can make to an API, providing a way to control access based on usage patterns. This can help prevent abuse and ensure the API remains available for all users.

**Settings:** Permissions can be configured globally through the DEFAULT_PERMISSION_CLASSES setting in settings.py, or on a per-view or per-viewset basis using the permission_classes attribute.

In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?

**Purpose**

The SELECT statement in SQL is used to retrieve data from one or more tables in a database. It allows the user to specify exactly which data they want to see, including:

*Which columns to include.

* Which rows to include, using the WHERE clause.
  
* How to sort the data, using the ORDER BY clause.
  
* Grouping of rows and applying aggregate functions, using the GROUP BY and HAVING clauses.
  
Retrieving All Columns from a Table

To retrieve all columns from a table called `employees`, you would use the following SQL statement:

```python
SELECT * FROM employees;

```

Here, * is a wildcard character that represents all columns in the table. This statement fetches every row from the employees table, returning all columns for each row.

This is a basic use of the SELECT statement, ideal for when you need to retrieve complete records from a table. For more complex queries, you can specify individual column names separated by commas, apply conditions to filter results, join tables, and more.

Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?

DRF's Generic Views are instrumental in building RESTful APIs efficiently. They encapsulate common functionality, reducing the amount of boilerplate code and allowing developers to focus on customizing their API's behavior rather than reinventing the wheel for basic CRUD operations. By leveraging these views, you can build a robust, scalable, and maintainable API with minimal effort.

**Concrete View Classes**

The following classes are the concrete generic views. If you're using generic views this is normally the level you'll be working at unless you need heavily customized behavior.

The view classes can be imported from rest_framework.generics.

**CreateAPIView**

Used for create-only endpoints.

Provides a post method handler.

Extends: GenericAPIView, CreateModelMixin

**ListAPIView**

Used for read-only endpoints to represent a collection of model instances.

Provides a get method handler.

Extends: GenericAPIView, ListModelMixin

**RetrieveAPIView**

Used for read-only endpoints to represent a single model instance.

Provides a get method handler.

Extends: GenericAPIView, RetrieveModelMixin

**DestroyAPIView**

Used for delete-only endpoints for a single model instance.

Provides a delete method handler.

Extends: GenericAPIView, DestroyModelMixin

**UpdateAPIView**

Used for update-only endpoints for a single model instance.

Provides put and patch method handlers.

Extends: GenericAPIView, UpdateModelMixin

**ListCreateAPIView**

Used for read-write endpoints to represent a collection of model instances.

Provides get and post method handlers.

Extends: GenericAPIView, ListModelMixin, CreateModelMixin

```python
from django.contrib.auth.models import User
from rest_framework import generics
from .models import Article
from .serializers import ArticleSerializer

class ArticleListCreate(generics.ListCreateAPIView):
    queryset = Article.objects.all()
    serializer_class = ArticleSerializer

```

**RetrieveUpdateAPIView**

Used for read or update endpoints to represent a single model instance.

Provides get, put and patch method handlers.

Extends: GenericAPIView, RetrieveModelMixin, UpdateModelMixin

**RetrieveDestroyAPIView**

Used for read or delete endpoints to represent a single model instance.

Provides get and delete method handlers.

Extends: GenericAPIView, RetrieveModelMixin, DestroyModelMixin

**RetrieveUpdateDestroyAPIView**

Used for read-write-delete endpoints to represent a single model instance.

Provides get, put, patch and delete method handlers.

Extends: GenericAPIView, RetrieveModelMixin, UpdateModelMixin, DestroyModelMixin

```python
class ArticleDetail(generics.RetrieveUpdateDestroyAPIView):
    queryset = Article.objects.all()
    serializer_class = ArticleSerializer

```

### Resources 

[Permissions](https://www.django-rest-framework.org/api-guide/permissions/)

[Review SQL Prework](https://chat.openai.com/)

[Generic views](https://www.django-rest-framework.org/api-guide/generic-views/)

[ChatGPT](https://chat.openai.com/)