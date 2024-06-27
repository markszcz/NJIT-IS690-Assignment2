## FastAPI and Pydantic

2. **Outline the complete process of handling a user login request in your FastAPI application. Provide a step-by-step explanation with code examples from the project.**

1) Go to localhost:8000/docs to gain access to the API
2) Register a test user in order to test he login. Go to the Login and Registration section and expand /register/
3) Click on the "Try it out" button, scroll down and press "Execute"
4) Scroll down and expand the /login/ section.
5) Click on the "Try it out" button.
6) Fill out the credentials john.doe@example.com/Secure*1234
7) Click on "Execute"
8) You can see the response down below.

The code the handles the login procedure can be found inthe /app/routers/user_routes.py file
- user_routes.py [user_routes](../app/routers/user_routes.py)