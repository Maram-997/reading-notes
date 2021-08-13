# Prep: Readings ... Get Ready for 401

## CallBacks:
* can be defined as a function that's called after somthing else happed
* most often CallBacks are sent in as arguements to another function; which then invokes the callback.
* the converstion goes like:
> " Function, do your work... and when you're done run this function for me."

#### Error First CallBacks:
There’s really only two rules for defining an error-first callback:

1. The first argument of the callback is reserved for an error object. If an error occurred, it will be returned by the first err argument.
2. The second argument of the callback is reserved for any successful response data. If no error occurred, err will be set to null and any successful data will be returned in the second argument.


## fs library : 
A library that allows us to read from the file system.

**Example**
`fs.readFile('/foo.txt', function(err, data) {
  // TODO: Error Handling Still Needed!
  console.log(data);
});`