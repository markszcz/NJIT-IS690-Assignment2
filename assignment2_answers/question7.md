## JWT and User Authentication

7. **Decode the following JWT and explain its contents:**
   - Token: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJqb2huLmRvZUBleGFtcGxlLmNvbSIsInJvbGUiOiJBRE1JTiIsInVzZXJfaWQiOiJjZGY4M2QzZi0zNzQ5LTRjZGQtOTRlYS1hNTVjZmMwNDhkMGYiLCJleHAiOjE3MTc2MTY4MjAuMjIwNzA5fQ.ANS8PgUiwPCmOvnZLYTCy_5WzLyhCDOx8aF4xu-Kaz8`
   - Use [jwt.io](https://jwt.io/) to decode and explain the contents.

Decoded:

Header:
{
  "alg": "HS256",
  "typ": "JWT"
}

alg: is the algorithm being used, HS256 encryption
typ: is the token type, in this case JWT

Payload:
{
  "sub": "john.doe@example.com",
  "role": "ADMIN",
  "user_id": "cdf83d3f-3749-4cdd-94ea-a55cfc048d0f",
  "exp": 1717616820.220709
}

The payload data is custom to the application,
sub:  The user/sub of the applkcation
rold: The role of the user
user_id: the unique ID, in this case GUID, of the user
exp: token expiration before being automatically invalidated based off of time.