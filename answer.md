# Answer These Questions Here, you can add additional pages to answer questions, just link to them so that I can view these questions and see your answer or the link(s) to your answer.

## FastAPI and Pydantic

1. **What role does Pydantic play in FastAPI, and how does it enhance data validation and settings management?**
   - Provide examples from the project where Pydantic is used.

- Question1 [Question1](./assignment2_answers/question1.md)

2. **Outline the complete process of handling a user login request in your FastAPI application. Provide a step-by-step explanation with code examples from the project.**

- Question2 [Question2](./assignment2_answers/question2.md)

3. **Explain the service repository pattern and how it is applied in your project. Provide an example of how routes are managed and linked to services.**

- Question3 [Question3](./assignment2_answers/question3.md)

## Database Management with Alembic and SQLAlchemy

4. **How does Alembic manage database migrations, and why is this important for maintaining database schemas?**
   - Illustrate with an example of a migration script from the project.

- Question4 [Question4](./assignment2_answers/question4.md)

## Pytest

5. **Why is Pytest critical for the development of the API?**
- Question5 [Question5](./assignment2_answers/question5.md)

## JWT and User Authentication

6. **Explain the functioning of JWT (JSON Web Tokens) in user authentication. How are JWTs generated, encoded, and used within the project?**
   - [Read this article and link to the code in the user management.](https://supertokens.com/blog/what-is-jwt)
   - Include a code snippet showing how JWTs are implemented in the project.
- Question6 [Question6](./assignment2_answers/question6.md)


7. **Decode the following JWT and explain its contents:**
   - Token: `eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJqb2huLmRvZUBleGFtcGxlLmNvbSIsInJvbGUiOiJBRE1JTiIsInVzZXJfaWQiOiJjZGY4M2QzZi0zNzQ5LTRjZGQtOTRlYS1hNTVjZmMwNDhkMGYiLCJleHAiOjE3MTc2MTY4MjAuMjIwNzA5fQ.ANS8PgUiwPCmOvnZLYTCy_5WzLyhCDOx8aF4xu-Kaz8`
   - Use [jwt.io](https://jwt.io/) to decode and explain the contents.
- Question7 [Question7](./assignment2_answers/question7.md)


8. **Describe the user registration logic in your project. Provide a pseudo-code workflow from the registration request to storing the user in the database.**
- Question8 [Question8](./assignment2_answers/question8.md)

9. **Detail the steps involved in the user email verification process. Provide a pseudo-code workflow from sending a verification email to activating the user's account.**
- Question9 [Question9](./assignment2_answers/question9.md)


## Security Practices

10. **How do you ensure the security of user passwords in your project? Discuss the hashing algorithm used and any additional security measures implemented.**
- Question10 [Question10](./assignment2_answers/question10.md)


11. **Explain the difference between hashing and encoding. Provide examples from your project where each is used:**
    - **Hashing:** Example and explanation with code
    - **Encoding:** Example and explanation with code
- Question11 [Question11](./assignment2_answers/question11.md)



## Project Management with Docker and CI/CD

12. **Discuss the advantages of using Docker Compose for running your project. How does it help in maintaining a consistent development and deployment environment?**
- Question12 [Question12](./assignment2_answers/question12.md)

13. **Describe the role of GitHub Actions in your project's CI/CD pipeline. How do you automate testing and deployment using GitHub Actions?**
- Question13 [Question13](./assignment2_answers/question13.md)


## API Design and Implementation

14. **What are REST APIs, and how do they function in your project? Provide an example of a REST endpoint from your user management system.**
- Question14 [Question14](./assignment2_answers/question14.md)


15. **What is HATEOAS (Hypermedia as the Engine of Application State)? Provide an example of its implementation in your project's API responses, along with a screenshot.**
- Question15 [Question15](./assignment2_answers/question15.md)


## Role-Based Access Control (RBAC)

16. **What is Role-Based Access Control (RBAC) and how is it implemented in your project?**
- Question16 [Question16](./assignment2_answers/question16.md)


17. **Explain the different user roles defined in your project (ANONYMOUS, AUTHENTICATED, MANAGER, ADMIN) and their permissions.**
- Question17 [Question17](./assignment2_answers/question17.md)

18. **Provide a code example showing how RBAC is enforced in one of your FastAPI endpoints.**
- Question18 [Question18](./assignment2_answers/question18.md)

## Route Parameters and Pydantic Schemas

19. **Explain how route parameters are used in FastAPI. Provide an example of a route that takes a parameter and demonstrate how it is used within the endpoint.**
- Question19 [Question19](./assignment2_answers/question19.md)

https://www.youtube.com/watch?v=jEA8tPKle6k&ab_channel=NavigateSuccesswithFirehose360 - 41:40 answer
The request goes to the route, the route then is just responsible , separateion of concerns, for taking the paramaters and passing it to the service thats actually going to do your business opperations (Business Logic) and the route prepares the response going back. The business operations are done in the service, not in the route. The service uses the schema, the pydantic schema, seriazliation and deserialization 


20. **How does FastAPI use Pydantic schemas to generate Swagger documentation? Provide an example from your project where a Pydantic schema is used and show the corresponding Swagger documentation.**
- Question20 [Question20](./assignment2_answers/question20.md)


These questions ensure a comprehensive assessment of the students' understanding of the topics related to your project setup, focusing on practical implementations and theoretical concepts.