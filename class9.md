#   Reading: Access Control (ACL)




When is Basic Authorization used vs. Bearer Authorization?
The Basic and Digest authentication schemes are dedicated to the authentication using a username and a secret.

The Bearer authentication scheme is dedicated to the authentication using a token. Even if this scheme comes from an OAuth2 specification, you can still use it in any other context where tokens are exchange between a client and a server.

What does the JSON Web Token package do?
JSON Web Token (JWT) is an open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed


What considerations should we make when creating and storing a SECRET?

1. JWTs used as Access Tokens

2. What algorithms to use


3. When to validate the token


4. Always check the issuer


5. Always check the audience

6. Make sure tokens are used as intended


7. Dealing with expiration, issued time and clock skew


8. How to work with the signature


9. When to use symmetric signing


