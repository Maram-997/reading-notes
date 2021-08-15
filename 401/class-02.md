# Read Class-02 : Express
## What’s the difference between PUT and PATCH?
**PUT**: The PUT method replaces all current representations of the target resource with the request payload.
**PATCH**: The PATCH method is used to apply partial modifications to a resource.
## Provide links to 3 services or tools that allow you to “mock” an API for development like json-server?

1. Postman Mock Server
2. Wiremock
3. Stoplight
 > **mocking tools fot http requests** :to imitates a real API server by providing realistic mock API responses to requests.
 > * A mock API server is useful during development and testing when live data is either unavailable or unreliable. so the absence of a real API doesn’t hold you back.

 ## Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?
 The easiest way to understand the difference is:
`OpenAPI = ***Specification***`
The OpenAPI is the official name of the specification. The development of the specification is fostered by the OpenAPI Initiative, which involves more the 30 organizations from different areas of the tech world — including Microsoft, Google, IBM, and CapitalOne. Smartbear Software, which is the company that leads the development of the Swagger tools, is also a member of the OpenAPI Initiative, helping lead the evolution of the specification.
`Swagger = ***Tools for implementing the specification***`
Swagger is the name associated with some of the most well-known, and widely used tools for implementing the OpenAPI specification. The Swagger toolset includes a mix of open source, free, and commercial tools, which can be used at different stages of the API lifecycle.
###### Which HTTP status codes should be sent with each type of (un)successful API call?
Successful: 200-status
unsuccessful : 400 or 500 depanding on the situation

## Compare and contrast SOAP and ReST:
1. **SOAP** 
* Simple Object Access Protocol
* protocol 
* needs more bandwidth for its usage
* only works with XML formats
* cannot make use of REST
2. **REST**
* Representational State Transfer
* architectural pattern
* doesn’t need much bandwidth 
* work with plain text, XML, HTML and JSON
* can make use of SOAP


## Document the following Vocabulary Terms
WEB SERVER: 
A web server is a computer that runs websites. It's a computer program that distributes web pages as they are requisitioned. The basic objective of the web server is to store, process and deliver web pages to the users. This intercommunication is done using Hypertext Transfer Protocol (HTTP).
EXPRESS:
Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.
ROUTING:
Defines the way in which the client requests are handled by the application endpoints. And when you make some routers in separate file, you can use them by using middleware.
