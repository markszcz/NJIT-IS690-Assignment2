## JWT and User Authentication

9. **Detail the steps involved in the user email verification process. Provide a pseudo-code workflow from sending a verification email to activating the user's account.**

1) Go to localhost:8000/docs to gain access to the API
2) Go to the Login and Registration section and expand /verify-email/{user_id}/{token}
3) Click on the "Try it out" button, fill out the user_id and token, then scroll down and press "Execute"
4) Within the code, we go to user_routes.py and follow the code for router.get for /verify-email/.
5) Within that code we await a response for the user service function verify_email_with_token()
6) Within the user_service module, we follow the logic to verify the token within the verify_email_with_token logic. 
7) The function calls a get_by_id by passing in the user_id to retrieve the record and the users token.
8) We check if the user even exists, and if so, compare the tokens.
9) If everything is ok, we commit the user to the database.