## FastAPI and Pydantic

3. **Explain the service repository pattern and how it is applied in your project. Provide an example of how routes are managed and linked to services.**

The service repository pattern is a pattern used to achieve a clean separation logic that should imporve maintanability and allow for easy compartmentalization of unit tests within the application. We can break down these patterns into repositories, services and pydantic models. 

For example we have to set up our user model, repository and service first before we use Fast API to route the endpoints. 
1) We create a user_model.py pydantic model. 
2) Then we create a user_schemasy.py respoistory.
3) Then we create the user_service.py service. 
Finally we can use all of this and route it in user_routes.py using FastAPI