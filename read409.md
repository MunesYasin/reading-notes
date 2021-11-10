# Access Control (ACL) 

## Vocabulary Terms 


* **encryption** Encryption is the process that scrambles readable text so it can only be read by the person who has the secret code, or decryption key. It helps provide data security for sensitive information.

* **token** Access tokens are the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user's data. Access tokens must be kept confidential in transit and in storage

* **bearer** Bearer authentication (also called token authentication) is an HTTP authentication scheme that involves security tokens called bearer tokens. ... The client must send this token in the Authorization header when making requests to protected resources: Authorization: Bearer <token>

* **secret** A generic term for any secret value that an attacker could use to impersonate the subscriber in an authentication protocol

* **JSON Web Token** JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed

## Review, Research, and Discussion 

**When is Basic Authorization used vs. Bearer Authorization?**

Bearer auth requires 2 calls, basic allows access directly with credentials.

**What does the JSON Web Token package do?** 

It is a library that contains authorization tools

**What considerations should we make when creating and storing a SECRET?** 

Where and how you are going to store it.

## Preview 

**Which 3 things had you heard about previously and now have better clarity on?**

* I have heard about the JSON Web Token package.
* I have heard about the Bearer Token.
* I have heard about the Basic Authorization.

**Which 3 things are you hoping to learn more about in the upcoming lecture/demo?**

* I am hoping to learn more about the JSON Web Token package.
* I am hoping to learn more about the Bearer Token.
* I am hoping to learn more about the Basic Authorization.

**What are you most excited about trying to implement or see how it works?**

* I am excited to see how the JSON Web Token package works.

## What is RBAC?
* **RBAC** is an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees,

* Benefits of RBAC:

1. Access control lists (ACL)
2. Attribute-based access control (ABAC)

## RBAC implementation

1. Inventory your systems
2. Analyze your workforce and create roles
3. Assign people to roles
4. Never make one-off changes
5. Audit

## Three primary rules are defined for RBAC

1. Role assignment: A subject can exercise a permission only if the subject has selected or been assigned a role.
2. Role authorization: A subject’s active role must be authorized for the subject. With rule 1 above, this rule ensures that users can take on only roles for which they are authorized.
3. Permission authorization: A subject can exercise a permission only if the permission is authorized for the subject’s active role. With rules 1 and 2, this rule ensures that users can exercise only permissions for which they are authorized.