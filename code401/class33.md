# Reading Notes

What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?

JSON Web Tokens (JWTs) serve as a compact, URL-safe means of representing claims to be transferred between two parties. JWTs do not encrypt the payload; they only encode it. While the payload is Base64Url encoded to be URL safe, it is easily decodable and should not contain sensitive information unless encrypted. The real security of a JWT comes from its ability to be verified and trusted through its digital signature.

How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?

JWT (JSON Web Tokens) Authentication in Django REST Framework (DRF) is a popular method for securing API endpoints. It ensures that only authenticated users can access certain views or perform specific actions. The integration process involves several key components and steps:

**Key Components**

* **JWT Library:** First, you need a library to handle JWT operations. In the Django ecosystem, libraries like djangorestframework-simplejwt or djangorestframework-jwt are commonly used. These libraries provide tools for generating, validating, and refreshing JWTs.

*  **User Model: **The default user model or a custom user model that Django uses to authenticate users.

* **Authentication and Permission Classes:** DRF uses these classes to control access to views. The JWT library provides an authentication class that you'll use to integrate JWT authentication.
  
* **Token Endpoint:** A dedicated endpoint for obtaining JWTs. Users provide their credentials (username and password) to this endpoint and receive a JWT if the credentials are valid.

* **Protected Endpoints:** The API endpoints you want to secure. Only requests with a valid JWT can access these endpoints.

Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?

Django's built-in development server, runserver, is designed for development purposes only and is not suitable for production environments due to several reasons

* **Performance:** The development server is single-threaded and not optimized for handling high volumes of traffic or concurrent requests efficiently, which are common in production environments.

* **Security:** runserver does not include security measures necessary to protect against various types of attacks that production servers need to withstand. It lacks the robustness in handling malicious traffic and does not enforce HTTPS, among other security features.

* **Features:** Production environments often require features such as serving static files efficiently, SSL/TLS support, load balancing, and the ability to handle multiple requests simultaneously. The Django development server does not provide these features.

* **Reliability:** The development server is not tested or designed to ensure the level of uptime and reliability expected in production environments.

**Gunicorn (Green Unicorn)** is a WSGI HTTP Server for UNIX, offering a simple and light interface for deploying Python web applications, including Django. It's widely used because it's easy to set up and works well with various web frameworks. Gunicorn is designed to handle concurrent connections and provides a simple, non-threaded worker model based on pre-forked workers.

### Resources

[JSON Web Tokens](https://jwt.io/introduction/)

[How to Use JWT Authentication with Django REST Framework](https://simpleisbetterthancomplex.com/tutorial/2018/12/19/how-to-use-jwt-authentication-with-django-rest-framework.html)

[Gunicorn 'Green Unicorn' ](https://gunicorn.org/)

[ChatGPT](https://chat.openai.com/)