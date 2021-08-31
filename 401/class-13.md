# Read - 13 : Message Queues
## What does it mean that web sockets are bidirectional? Why is this useful?
Whereas HTTP relies on a client request to receive a response from the server for every exchange, WebSockets allow for full-duplex bidirectional communication. This enables the server to send real-time updates asynchronously, without requiring the client to submit a request each time.

## Does socket.io use HTTP? Why?
Even when websockets can be used, the initial connection setup it done over HTTP. Also, a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js .

## What happens when a client emits an event?
It sholud be heard on the server side as well.

## What happens when a server emits an event?
It can be heard on any client server.

##  What happens if a client “misses” an event?
ignored. It's just like when an event occurs and there are no event listeners for that event. The socket receives the msg and doesn't find a handler for it so nothing happens with it.

## How can we mitigate this?
Through using the queues.
