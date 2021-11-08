# Code 401 Class 08 Reading notes:

## Review, Research, and Discussion

### When is Basic Authorization used vs. Bearer Authorization?

The HOPEX REST API based on GraphQL allows to be called in two way :

With a Basic Auth
With Bearer Token
Depending on the use case you want to use the API you may use one or the other.

Regardless of the chosen authentication methods the others headers and body information will remains the same.
### What does the JSON Web Token package do?
Allows you to use JSON Web Tokens to securely transfer data between two parties as JSON objects
### What considerations should we make when creating and storing a SECRET?
- a secret should be secure
- secrets should be encrypted
- secret should be visually different from id
## Document the following Vocabulary Terms

**encryption**

Cryptographically turns data into a secret code that cannot easily be deciphered

**token**

A token is a thing that represents an object

**bearer**

A type of token used for authentication - represents the user

**secret**

A secret ket or passcode used to login or create a login/token

**JSON Web Token**

JSON web tokens are used to securely transmit data between parties as 
JSON objects

## Preview

### Which 3 things had you heard about previously and now have better clarity on?
- Jest
- Jwt
- Base-64
### Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
- RBAC
- EDA
- AWS
### What are you most excited about trying to implement or see how it works?
Authorising user to access certain data only after signing in, allowing user to change/password.

## Preparation Materials
### RBAC
RBAC is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.
### 5 steps to simple role-based access control (RBAC)

1. Inventory your systems
Figure out what resources you have for which you need to control access, if you don't already have them listed. 

2. Analyze your workforce and create roles
You need to group your workforce members into roles with common access needs.  Avoid the temptation to have too many roles defined. Keep them as simple and stratified as possible.

3. Assign people to roles
Now that you have a list of roles and their access rights, figure out which role(s) each employee belongs in, and set their access accordingly. 

4. Never make one-off changes
Resist any temptation to make a one-off change for an employee with unusual needs. If you begin doing this, your RBAC system will quickly begin to unravel. Change the roles as required or add new ones when really necessary.

5. Audit
Periodically review your roles, the employees assigned to them, and the access permitted for each. If you discover, for example, that a role has unnecessary access to a particular system, change the role and adjust the access level for all employees in that role. 
#### Want To Know More ? 
- [RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)
- [5 steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)
- [wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)