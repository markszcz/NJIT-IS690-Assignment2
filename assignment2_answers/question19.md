## Route Parameters and Pydantic Schemas

19. **Explain how route parameters are used in FastAPI. Provide an example of a route that takes a parameter and demonstrate how it is used within the endpoint.**
Each endpoint can recieve paramanters, but Paramanters that are passed into an API have to be explicitly catpured in the router in order to be used. 
For example the {user_id} for get users in user_routes.py on line 26:
```
@router.get(
            "/users/{user_id}", 
```

on line 36, the API knows to take that input paramater so it can them be passed over to get_by_id() function. 
 
```
user = await UserService.get_by_id(db, user_id)
``` 