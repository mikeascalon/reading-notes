# Reading Notes

## What does REST stand for?

Representational State Transfer (REST) as an architectural approach to designing web services.

REST APIs are designed around a ____.

Resourses

What is an identifier of a resource? Give an example.

An identifier of a resource, often referred to as a Uniform Resource Identifier (URI), is a string of characters used to identify a particular resource on the internet.

```html
https://adventure-works.com/orders/1
```

What are the most common HTTP verbs?

The most common operations are GET, POST, PUT, PATCH, and DELETE.

What should the URIs be based on?

Try to keep URIs relatively simple. Once an application has a reference to a resource, it should be possible to use this reference to find items related to that resource and try to avoid "chatty" web APIs that expose a large number of small resources.

Give an example of a good URI.

```html
https://www.example.com/products/electronics/smartphones/iphone-13
```

What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

the key is to strike a balance between granularity and efficiency. While some applications benefit from chatty APIs due to granular Contro and Reduced Data Transfer:, others may prefer coarser-grained APIs to minimize network overhead and improve performance. The suitability of a chatty API depends on the specific requirements and constraints of the application using it.

What status code does a successful GET request return?

200

What status code does an unsuccessful GET request return?

400s and 500s

What status code does a successful POST request return?

201

What status code does a successful DELETE request return?

204

### Resourses

[RESTful web API design](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)

[ChatGPT](https://chat.openai.com/)
