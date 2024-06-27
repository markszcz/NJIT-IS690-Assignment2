## FastAPI and Pydantic

1. **What role does Pydantic play in FastAPI, and how does it enhance data validation and settings management?**
   - Provide examples from the project where Pydantic is used.

Pydantic is a Python library to help create APIs. These are schemas that helps with data validation, parising and its searialization capabilities help ensure the applciations data is in the correct format. It also can help convert different data formats such as JSON into Python objects.

Examples from the project could be found in the app/schemas folder:
- event_schema.py [event_schema](../app/schemas/event_schema.py)
- link_schema.py [link_schema](../app/schemas/link_schema.py)
- pagination_schema.py [pagination_schema](../app/schemas/pagination_schema.py)
- token_schema.py [token_schema](../app/schemas/token_schema.py)
- user_schemas.py [user_schemas](../app/schemas/user_schemas.py)
