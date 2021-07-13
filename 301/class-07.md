# Read : Class 07 - REST:

## Who is Roy Fielding:
one of the principal authors of the HTTP specification and the originator of the Representational State Transfer (REST) architectural style.
> What He did:
> 1. He helped write the first web servers, that sent documents across the internet. 
> 2. and then he did a ton of research explaining why the web works the way it does.

## Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world:
 We need to be able to talk to all machines about all the stuff that's on all the other machines. So we need some way of having one machine tell another machine about a resource that might be on yet another machine.
 * **On the internet, it's called a "redirect"**

 ## What is an identifer of a resource? Give an example:
 The target of an HTTP request is called a "resource", whose nature isn't defined further; it can be a document, a photo, or anything else. Each resource is identified by a Uniform Resource Identifier (URI) used throughout HTTP for identifying resources.
`www.example.com`

## What are the most common HTTP verbs:
The most common operations are GET, POST, PUT, PATCH, and DELETE.

## What should the URIs be based on:
resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

## Give an example of a good URI.
https://adventure-works.com/`orders` // Good

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing:
try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request.


 ## So how do the machines tell each other where things are:
 With a URL. If everything that machines need to talk about has a corresponding URL, you've created the machine equivalent of a noun. That you and I and the rest of the world have agreed on talking about nouns in a certain way is pretty important.

 ## What is the HTTP protocol that Fielding and his friends created:
 **The Hypertext Transfer Protocol** (HTTP) is an application layer protocol for `distributed`, `collaborative`, `hypermedia information systems`. **HTTP** is the foundation of data communication for the World Wide Web, where hypertext documents include hyperlinks to other resources that the user can easily access.

 #### What does a **GET** do: 
 The GET method requests that the target resource transfers a representation of its state. GET requests should only retrieve data and should have no other effect.
 #### What does a **POST** do:
 The POST method requests that the target resource processes the representation enclosed in the request according to the semantics of the target resource.
 #### What does **PUT** do:
 The PUT method requests that the target resource creates or updates its state with the state defined by the representation enclosed in the request.
 #### What does **PATCH** do:
 The PATCH method requests that the target resource modifies its state according to the partial update defined in the representation enclosed in the request.

Geocoding API
Did you get your API key? **yes** 
Weather Bit API
Did you get your API key? **yes** 
Yelp API Docs
Did you get your API key? **no** 
The Movie DB API Docs
Did you get your API key? **yes**