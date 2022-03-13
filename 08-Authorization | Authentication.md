
# Review, Research, and Discussion

1- What header(s) are used in authentication and authorization?
The HTTP Authorization request header can be used to provide credentials that authenticate a user
agent with a server, allowing access to a protected resource. The Authorization header is usually, but not always, sent after the user agent
first attempts to request a protected resource without credentials.


2- What is safe to put into a JWT ?
 verifiable security statements, such as the identity of the user
 
3 -How are JWTs validated?

 JWTs are signed so they can't be modified in transit. When an authorization server issues a token, it signs it using a key. 
 When the client receives the ID token, the client validates the signature using a key as well.
 

# Vocabulary Terms

RBAC =>Role-based access control (RBAC) is a method of restricting network access based on the roles of individual users within an enterprise.

User Roles => User Roles are permission sets that control access to areas and features within the Professional Archive Platform.
Each User account requires a Role assignment.

JWT Token => JWT, or JSON Web Token, is an open standard used to share security information between two parties — a client and a server. 
Each JWT contains encoded JSON objects, including a set of claims
