## JWT and User Authentication

6. **Explain the functioning of JWT (JSON Web Tokens) in user authentication. How are JWTs generated, encoded, and used within the project?**
   - [Read this article and link to the code in the user management.](https://supertokens.com/blog/what-is-jwt)
   - Include a code snippet showing how JWTs are implemented in the project.

JWT is an open standard of sending secure transmission of data between parties in JSON format. One way of using JWT is for user authentication. 

When a user logs into a web page, the credentials are sent to the backender server. The server validates the login and if the credentials are valid, creats a JWT. The JWT has three parts: 
1) The Header: which defines the signing algorithm used
2) The Payload: which contains the user information encoded in JSON format
3) The Signature: signature of the header and payload using a secret key known only by the sever.

The JWT is then sent to the client to be stored in its session cookie. Any subsequent request always includes the JWT that the server an easily verify as proof the user was previously authenticated. The backend server recieves the JWT and validates the signature to the message.

The code within the project to do this logic can be located:
- jwt_service.py [jwt_service](../app/services/jwt_service.py)
