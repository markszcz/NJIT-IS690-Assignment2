## Security Practices

11. **Explain the difference between hashing and encoding. Provide examples from your project where each is used:**
    - **Hashing:** Example and explanation with code
    - **Encoding:** Example and explanation with code

Hashing is when you need to verify data integrity, or create a secure represenation such as passwords. This is usally a one way methond.
Encoding is when you need to transform data for a specific purpose, for example transforming data into JSON format. This is a reversible method. 

Hashing example is when we hashed the password to be stored in the database:
Line 51 in user_services.py.  
validated_data['hashed_password'] = hash_password(validated_data.pop('password'))

Encoding example is when we need to create the access token in JSON.
Line 207-210 in user_routes.py 
access_token = create_access_token(
    data={"sub": user.email, "role": str(user.role.name), "user_id": str(user.id)},
    expires_delta=access_token_expires
)