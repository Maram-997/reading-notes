# Read : Class 08 - APIs

## APIs: 
A RESTful API is an architectural style for an application program interface (API) that uses HTTP requests to access and use data. That data can be used to GET, PUT, POST and DELETE data types, which refers to the reading, updating, creating and deleting of operations concerning resources.
>* An API for a website is code that allows two software programs to communicate with each other.
>* The API spells out the proper way for a developer to write a program requesting services from an operating system or other application.
>* A RESTful API is based on representational state transfer (REST), which is an architectural style and approach to communications often used in web services development.

  ## REST:
REST, or **REpresentational State Transfer**, is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other. REST-compliant systems, often called RESTful systems, are characterized by how they are stateless and separate the concerns of client and server. We will go into what these terms mean and why they are beneficial characteristics for services on the Web.

> By using a REST interface, different clients hit the same REST endpoints, perform the same actions, and receive the same responses.

**Statelessness**
Systems that follow the REST paradigm are stateless, meaning that the server does not need to know anything about what state the client is in and vice versa. In this way, both the server and the client can understand any message received, even without seeing previous messages. This constraint of statelessness is enforced through the use of resources, rather than commands. Resources are the nouns of the Web - they describe any object, document, or thing that you may need to store or send to other services.

> Because REST systems interact through standard operations on resources, they do not rely on the implementation of interfaces.

These constraints help RESTful applications achieve reliability, quick performance, and scalability, as components that can be managed, updated, and reused without affecting the system as a whole, even during operation of the system.

**Communication between Client and Server**
In the REST architecture, clients send requests to retrieve or modify resources, and servers send responses to these requests. Let’s take a look at the standard ways to make requests and send responses.

 **Making Requests**
REST requires that a client make a request to the server in order to retrieve or modify data on the server. A request generally consists of:


#### There are 4 basic HTTP verbs we use in requests to interact with resources in a REST system:

GET — retrieve a specific resource (by id) or a collection of resources
POST — create a new resource
PUT — update a specific resource (by id)
DELETE — remove a specific resource by id

## The maturity model for web APIs 
The Richardson Maturity Model (RMM) is a maturity model suggested in 2008 by
 Leonard Richardson which classifies Web APIs based on their adherence and
 conformity to each of the model's four levels

 ## Organize the API design around resources 
 Most modern web applications expose APIs that clients can use to interact with the application. A well-designed web API should aim to support:

1. Platform independence. Any client should be able to call the API, regardless of how the API is implemented internally. This requires using standard protocols, and having a mechanism whereby the client and the web service can agree on the format of the data to exchange.

2. Service evolution. The web API should be able to evolve and add functionality independently from client applications. As the API evolves, existing client applications should continue to function without modification. All functionality should be discoverable so that client applications can fully use it.
