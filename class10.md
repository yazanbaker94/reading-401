What header(s) are used in authentication and authorization
The Authorization and Proxy-Authorization request headers contain the credentials to authenticate a user agent with a (proxy) server. Here, the <type> is needed again followed by the credentials, which can be encoded or encrypted depending on which authentication scheme is used
  
  
What is safe to put into a JWT
  
  A JWT needs to be stored in a safe place inside the user's browser. ... To keep them secure, you should always store JWTs inside an httpOnly cookie. This is a special kind of cookie that's only sent in HTTP requests to the server. It's never accessible (both for reading or writing) from JavaScript running in the browser
  
How are JWTs validated
  
  Check signature. The last segment of a JWT is the signature, which is used to verify that the token was signed by the sender and not altered in any way. The Signature is created using the Header and Payload segments, a signing algorithm, and a secret or public key (depending on the chosen signing algorithm
  
  RBAC
  
  
Role-based access control (RBAC) is a method of restricting network access based on the roles of individual users within an enterprise. RBAC lets employees have access rights only to the information they need to do their jobs and prevents them from accessing information that doesn't pertain to them.
  
  
User Roles
  
  A user role defines permissions for users to perform a group of tasks. In a default WordPress installation there are some predefined roles with a predefined set of permissions. These roles are Super Admin, Administrator, Editor, Author, Contributor, and Subscriber.
  
  
JWT Token
  
  JSON Web Token (JWT) is a JSON encoded representation of a claim(s) that can be transferred between two parties. The claim is digitally signed by the issuer of the token, and the party receiving this token can later use this digital signature to prove the ownership on the claim.
