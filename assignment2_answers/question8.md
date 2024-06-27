## JWT and User Authentication

8. **Describe the user registration logic in your project. Provide a pseudo-code workflow from the registration request to storing the user in the database.**


1) Go to localhost:8000/docs to gain access to the API
2) Go to the Login and Registration section and expand /register/
3) Click on the "Try it out" button, scroll down and press "Execute"
4) Within the code, we go to user_routes.py and follow the code for router.post for /register/.
5) The code then executes the await UserServices.register_user() function.
6) Following that down the stack, the register_user function in user_services.py file then calls the create() function.
7) Within the create() function, after some validation for duplicate users, and hashing the pasword, it adds a new_user to the session and commits the changes.
