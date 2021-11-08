# Code 401 Class 07 Reading notes:

## Review, Research, and Discussion

### Write the following steps in the correct order:

1. Register your application to get a client_id and client_secret
2. Ask the client if they want to sign in via a third party
3. Redirect to a third party authentication endpoint
4. Receive access token
5. Make a request to the access token endpoint
6. Receive authorization code
7. Make a request to a third-party API endpoint


### What can you do with an authorization code?
see what the information the client is requesting, and approve or deny the request, exchange for an access token

### What can you do with an access token?
use to make API requests
### What’s a benefit of using OAuth instead of your own basic authentication?
With Basic authentication the full credentials are always included in each request, while with OAuth it's the access token that is included in each request.


### Document the following Vocabulary Terms

**Client ID**

The client_id is a public identifier for apps, It must also be unique across all clients that the authorization server handles.

**Client Secret**

The client_secret is a secret known only to the application and the authorization server. It must be sufficiently random to not be guessable.

**Authentication Endpoint**

mechanism used to verify the identity of a network's connecting device .

**Access Token Endpoint**

used in token-based authentication to allow an application to access an API .


**API Endpoint**

is the point of communication when two systems are interacting. It refers to communication between an API and a server.

**Authorization Code**

is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server

**Access Token**

used in token-based authentication to allow an application to access an API .


## Preview


### Which 3 things had you heard about previously and now have better clarity on?
- base64
- authentication 
- authorization
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- JWT
- socket IO
- Reviewing db though heroku
### What are you most excited about trying to implement or see how it works?
Fully functioning app with all new concepts learned using the best practices.

## Preparation Materials

### Intro to JWT
JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.
### When should you use JSON Web Tokens?
- Authorization: 

This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.

- Information Exchange: 

JSON Web Tokens are a good way of securely transmitting information between parties. Because JWTs can be signed—for example, using public/private key pairs—you can be sure the senders are who they say they are. 
### Are JWTs Secure?

JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.
### What is the JSON Web Token structure?

In its compact form, JSON Web Tokens consist of three parts separated by dots (.), which are:

- Header
- Payload
- Signature

Therefore, a JWT typically looks like the following.

xxxxx.yyyyy.zzzzz

### Bookmark

- [npm jsonwebtoken docs](https://www.npmjs.com/package/jsonwebtoken)
#### Want To Know More ? 
- [JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)
- [Intro to JWT](https://canvas.instructure.com/courses/3671271/discussion_topics/12904449)
- [Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)