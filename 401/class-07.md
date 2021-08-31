# Read - 07 : Bearer Authorization
## Write the following steps in the correct order:
1. Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Make a request to a third-party API endpoint
4. Redirect to a third party authentication endpoint
5. Make a request to the access token endpoint
6. Receive access token
7. Receive authorization code

## What can you do with an authorization code?
An authorization code is an alphanumeric password that authorizes its user to purchase, sell or transfer items, or to enter information into a security-protected space

## What can you do with an access token?
An access token is an opaque string that identifies a user, app, or Page and can be used by the app to make graph API calls. When someone connects with an app using Facebook Login and approves the request for permissions, the app obtains an access token that provides temporary, secure access to Facebook APIs.

## What’s a benefit of using OAuth instead of your own basic authentication?
It enables apps to obtain limited access (scopes) to a user's data without giving away a user's password. It decouples authentication from authorization and supports multiple use cases addressing different device capabilities. It supports server-to-server apps, browser-based apps, mobile/native apps, and consoles/TVs.