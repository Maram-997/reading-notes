# Read - 08 : Access Control (ACL)
## When is Basic Authorization used vs. Bearer Authorization?
The Basic authentication schemes are dedicated to the authentication using a username and a secret. The Bearer authentication scheme is dedicated to the authentication using a token.

## What does the JSON Web Token package do?
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

## What considerations should we make when creating and storing a SECRET?
1. Never store unencrypted secrets in .git repositories
2. Don’t share your secrets unencrypted in messaging systems like slack
3. Store secrets safely
4. Restrict API access and permissions