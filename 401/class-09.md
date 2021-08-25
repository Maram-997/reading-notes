# Read - 09 : 
## What header(s) are used in authentication and authorization?
The WWW HTTP request headers contain the credentials to authenticate a user agent with a (proxy) server. Here, the `<type>` is needed again followed by the credentials, which can be encoded or encrypted depending on which authentication scheme is used.

## What is safe to put into a JWT?
JWTs used as Access Tokens; This means that they contain data. 

## How are JWTs validated?
To validate a JWT, your application needs to:
1. Check that the JWT is well formed.
2. Check the signature.
3. Check the standard claims.
> If any of these steps fail, then the associated request must be rejected.
A well-formed JWT consists of three concatenated Base64url-encoded strings, separated by dots (.):

1. JOSE Header: contains metadata about the type of token and the cryptographic algorithms used to secure its contents.
2. JWS payload (set of claims): contains verifiable security statements, such as the identity of the user and the permissions they are allowed.
3. JWS signature: used to validate that the token is trustworthy and has not been tampered with. When you use a JWT, you must check its signature before storing and using it.

A JWT typically looks like this:
![img](https://images.ctfassets.net/cdy7uua7fh8z/7FI79jeM55zrNGd6QFdxnc/80a18597f06faf96da649f86560cbeab/encoded-jwt3.png)