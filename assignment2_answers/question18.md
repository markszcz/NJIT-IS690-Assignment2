## Role-Based Access Control (RBAC)

18. **Provide a code example showing how RBAC is enforced in one of your FastAPI endpoints.**

In the event_routes.py file, when calling a function a paramater that is passed in requires a check that the users role is either and ADMIN or MANAGER.
```current_user: dict = Depends(require_role(["ADMIN", "MANAGER"])))```

For example line 20 in event_routes.py
- event_routes.py [event_routes](../app/routers/event_routes.py)