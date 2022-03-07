# JWT
JWT, or JSON Web Token, is an open standard used to share security information between two parties — a client and a server. Each JWT contains encoded JSON objects,
including a set of claims. JWTs are signed using a cryptographic algorithm to ensure that the claims cannot be altered after the token is issued.

## How JWT Works
JWTs differ from other web tokens in that they contain a set of claims. Claims are used totransmit information between two parties. What these claims are depends 
on the use case at hand. For example, a claim may assert who issued the token, how long it is valid for, or what permissions the client has been granted.
A JWT is a string made up of three parts, separated by dots (.), and serialized using base64. In the most common serialization format,
compact serialization, the JWT looks something like this: xxxxx.yyyyy.zzzzz. Once decoded, you will get two JSON strings:

   - The header and the payload.
   - The signature. 

The JOSE (JSON Object Signing and Encryption) header contains the type of token — JWT in this case — and the signing algorithm.  The payload contains the claims. 
This is displayed as a JSON string, usually containing no more than a dozen fields to keep the JWT compact. This information is typically used by the server 
to verify that the user has permission to perform the action they are requesting.There are no mandatory claims for a JWT, but overlaying standards may make claims 
mandatory. For example, when using JWT as bearer access token under OAuth2.0, iss, sub, aud, and exp must be present. some are more common than others. The signature 
ensures that the token hasn’t been altered. The party that creates the JWT signs the header and payload with a secret that is known to both the issuer and receiver,
or with a private key known only to the sender. When the token is used, the receiving party verifies that the header and payload match the signature. 

# Vocabulary Terms

Client ID => is an identifier associated with an application that assists with client
Client Secret => is a secret used by the OAuth Client to Authenticate to the Authorization Server
Authentication Endpoint => is a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.
Access Token Endpoint =>is where apps make a request to get an access token for a user.
API Endpoint => is a point at which an API -- the code that allows two software programs to communicate with each other -- connects with the software program.
Authorization Code =>  is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user
gets a chance to see what the information the client is requesting, and approve or deny the request
Access Token => Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific
application to access specific parts of a user's data.



