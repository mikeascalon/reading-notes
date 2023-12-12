# Reading Notes

## In your own words, describe what each group of status code represents

100’s = this code is when the server is busy and can't send the body requested.

200’s = this code when the server was sucessfully send back to the client what was requested.

300’s = this error occurs when the client's requested information is not on the server.

400’s = this error is a client error where it can be a syntax error,  or a bad API Url. Server did not understand or cannot process the request you sent.

500’s = it means that the server, which is the computer that hosts the website, encountered a problem while trying to fulfill your request.

What is a status code 202?

it's essentially saying, "I've received your request, and I'm working on it, but I'm not done yet."

What is a status code 308?

The resource you're looking for has moved permanently, and you need to use this new address to find it.

What code would you use if an update didn’t return data to a client?

204 No Content

What code would you use if a resource used to exist but no longer does?

404 Not Found

What is the ‘Forbidden’ status code?

HTTP status code 403.

Why do we need to pull our MongoDB database string out of our server and put it into our .env?

Storing sensitive information, such as database connection strings, in a separate configuration file helps improve security.

What is middleware?

Middleware is a type of computer software that provides services to software applications beyond those available from the operating system

What does app.use(express.json()) do?

The app.use(express.json()) function in Express is a built-in middleware function that parses incoming requests with JSON payloads and is based on body-parser. It returns middleware that only parses JSON and populates the parsed data in req.body.

What does the /:id mean in a route?

The /:id in a route is a route parameter in Express. It is used to capture values at a specific position in the URL. When a request is made to a route that contains /:id, the value specified in that position in the URL is captured and can be accessed via req.params.id.

What is the difference between PUT and PATCH?

PUT is used to update or create a resource by sending all the resource parameters, while PATCH is used to partially update an existing resource by sending only the fields that need to be updated.

How do you make a default value in a schema?

In Mongoose, you can set a default value in a schema using the default keyword. When defining a schema, you can specify the default value for a field. If a new document is created without a value for that field, the default value will be used.

What does a 500 error status code mean?

The 500 error status code, specifically the "500 Internal Server Error," indicates that the server encountered an unexpected condition that prevented it from fulfilling the request.

What is the difference between a status 200 and a status 201?

the 200 status code is a general success response, while the 201 status code specifically indicates that a new resource has been successfully created as a result of the request.

### Resources

[Which HTTP Status Code to Use for Every CRUD App](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

[ChatGPT](https://chat.openai.com/)
