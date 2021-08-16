# Read Class-03 : Express REST API
## Name 3 real world use cases where you’d want to change the request with custom middleware:
1. Request Tracker.
2. Controls how application responds to HTTP requests.
3. Control how application looks when there is an error.

## True or false: The route handler is middleware? (FALSE)
They are not middleware functions by definition. If such function is used on routing methods then they are only handler functions.

## In what ways can a middleware function end the process and send data to the browser?
* Ending the Process => By sending the response.
* when we next() with a message.

## At what point in the request lifecycle can you “inject” middleware?
when we creating the middleware for response to send it.
![img](https://imgs.developpaper.com/imgs/399369332-5e37a5e9724f6_articlex.png)

## What can cause express to error with “Request headers sent twice, cannot start a second response”
means that you're already in the Body or Finished state, but some function tried to set a header or statu. 