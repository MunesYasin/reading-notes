# Authorization/Authentication 

## Review, Research, and Discussion 

**What header(s) are used in authentication and authorization**

* The WWW-Authenticate and Proxy-Authenticate response headers define the authentication method that should be used to gain access to a resource. They must specify which authentication scheme is used, so that the client that wishes to authorize knows how to provide the credentials.

**What is safe to put into a JWT**
* add "secret" that is used to generate the JWT. If someone modifies the data contained in the JWT, the server will fail to decode it. So the server can trust any JWT that it can decode.

**How are JWTs validate**

* the server validates the username and password combination and creates a JWT token with a payload containing the user technical identifier and an expiration timestamp.

## Terms

* **RBAC**:Role-based access control is a method of restricting network access based on the roles of individual users within an enterprise.

* **User Roles**: are permission sets that control access to areas and features within the Professional Archive Platform. Each User account requires a Role assignment.

* **JWT Token**: (JSON Web Token (JWT) access tokens conform to the JWT standard and contain information about an entity in the form of claims. They are self-contained therefore it is not necessary for the recipient to call a server to validate the token.

## Preview 

**Which 3 things had you heard about previously and now have better clarity on?**

* User Role
* authentication & authorization
* Access Token

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* basic Authorization s
* JWT.
* Bearer Authorization

**What are you most excited about trying to implement or see how it works?**

* more about access control using CRUD function