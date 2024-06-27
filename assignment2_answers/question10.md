## Security Practices

10. **How do you ensure the security of user passwords in your project? Discuss the hashing algorithm used and any additional security measures implemented.**

A hashing algorithm is a one-way crpytographic function designed specificlly to securely store passwords. In the event of a data breach, passwords "should not" become compromised. 

The user passwords use the python bcrypt library in order to hash the users password. This logic is done in the user_services.py file under the create function.
Line 51: validated_data['hashed_password'] = hash_password(validated_data.pop('password'))
- user_service.py [user_service](../app/services/user_service.py)
