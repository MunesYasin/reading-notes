# Bearer Authorization 

## Client ID
At registration the client application is assigned a client ID and a client secret (password) by the authorization server. The client ID and secret is unique to the client application on that authorization server. ... This redirect URI is used when a resource owner grants authorization to the client application

## Authentication Endpoint
An authorization endpoint is an HTTP endpoint that micropub and IndieAuth clients can use to identify a user or obtain an authorization code (which is then later exchanged for an access token) to be able to post to their website

## Access Token Endpoint
Access tokens are the thing that applications use to make API requests on behalf of a user. ... The token endpoint is where apps make a request to get an access token for a user. This section describes how to verify token requests and how to return the appropriate response and errors

## API Endpoint
Simply put, an endpoint is one end of a communication channel. When an API interacts with another system, the touchpoints of this communication are considered endpoints. For APIs, an endpoint can include a URL of a server or service

## Authorization Code
The authorization code is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request

## Access Token
Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage

## Review, Research, and Discussion 

**Write the following steps in the correct order :**

* Register your application to get a client_id and client_secret
* Ask the client if they want to sign in via a third party
* Make a request to a third-party API endpoint
* Make a request to the access token endpoint
* Receive access token
* Redirect to a third party authentication endpoint
* Receive authorization code

**What can you do with an authorization code?**

* to authentic a user or to authorize a user get certain information.

**What can you do with an access token?**

 to give secure authorization.

**What’s a benefit of using OAuth instead of your own basic authentication?**

 it is stronger.

 ## Preview 

 **Which 3 things had you heard about previously and now have better clarity on?**

* inserted on Linked list
* authentication & authorization
* Access Token

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* JWT.
* auth0.
* Bearer Authorization

**What are you most excited about trying to implement or see how it works?**

* JWT

## JWTs Explained

**What is JSON Web Token?**

*JSON Web Token* (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.

## Intro to JWT
**Why should we use JSON Web Tokens?**

Let’s talk about the benefits of JSON Web Tokens (JWT) when compared to Simple Web Tokens (SWT) and Security Assertion Markup Language Tokens (SAML).

As JSON is less verbose than XML, when it is encoded its size is also smaller, making JWT more compact than SAML. This makes JWT a good choice to be passed in HTML and HTTP environments.

Security-wise, SWT can only be symmetrically signed by a shared secret using the HMAC algorithm. However, JWT and SAML tokens can use a public/private key pair in the form of a X.509 certificate for signing. Signing XML with XML Digital Signature without introducing obscure security holes is very difficult when compared to the simplicity of signing JSON.

## Are JWTs Secure?
JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don’t know the private key, you can’t change it. Otherwise, the receiver will notice that the signature won’t match anymore.

Answer to your comment: I’m not sure if I understand your comment the right way. Just to be sure: do you know and understand digital signatures? I’ll just briefly explain one variant (HMAC, which is symmetrical, but there are many others).

Let’s assume Alice wants to send a JWT to Bob. They both know some shared secret. Mallory doesn’t know that secret, but wants to interfere and change the JWT. To prevent that, Alice calculates Hash(payload + secret) and appends this as signature.