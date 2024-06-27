## Role-Based Access Control (RBAC)

17. **Explain the different user roles defined in your project (ANONYMOUS, AUTHENTICATED, MANAGER, ADMIN) and their permissions.**

There are two category of roles that are used in the application.
Implicit roles are ANONYMOUS, AUTHENTICATED
Assigned roles are MANAGER, ADMIN

Implicit roles:
The difference between these two groups utilize two different sets of logic. For example anyone with an "ANONYMOUS" role is implicitly not logged into the appliction and also the backend server does not know who the user is. The only logical API that the user has access to is the Login and Register API. 

The "AUTHENTICATED" role is anyone who has a successful token due to a correct login. They are implicitly understood to be an authenticated user based on that fact and we are nout putting in explicit logic to check if a users role = "AUTHENTICATED". These type of users have access to get and update their account.

Assigned roles:
These roles are assigned to a user, usually stored in their "roles" attribute and are explicitly checked for within the code. There will be logic to check if .role = "MANAGER or ADMIN" These individuals would have access to access the rest of the API in the application, but with varying authorization based on their Role.