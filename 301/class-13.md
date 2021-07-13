# Read : Class 13 - CRUD

## Status Code 
it's a part of the response returned by the server when a client (e.g., a browser) calls a URL. With the help of a status code, the server tells the client whether the request was successfully processed or whether an error occurred.
* 100s = Information responses
* 200s = Successful responses 
* 300s = Redirection messages
* 400s = Client error responses
* 500s = Server error responses 


## QUES:
#### What is a status code 202:
**202 Accepted**
The request has been received but not yet acted upon. It is noncommittal, since there is no way in HTTP to later send an asynchronous response indicating the outcome of the request. It is intended for cases where another process or server handles the request, or for batch processing.
#### What is a status code 308:
**308 Permanent Redirect**
This means that the resource is now permanently located at another URI, specified by the Location: HTTP Response header. This has the same semantics as the 301 Moved Permanently HTTP response code, with the exception that the user agent must not change the HTTP method used: If a POST was used in the first request, a POST must be used in the second request.
#### What code would you use if an update didn’t return data to a client:
 400s => Client error responses

#### What code would you use if a resource used to exist but no longer does:
404 - Not Found 
#### What is the ‘Forbidden’ status code:
**403 Forbidden**
The client does not have access rights to the content; that is, it is unauthorized, so the server is refusing to give the requested resource. Unlike 401, the client's identity is known to the server.