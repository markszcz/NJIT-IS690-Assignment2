## Project Management with Docker and CI/CD

12. **Discuss the advantages of using Docker Compose for running your project. How does it help in maintaining a consistent development and deployment environment?**

Utilizing docker compose allows us to maintain a consistend development and deployment environment. When it comes to consistend development environmnents, docker allows us to remove any discrepencies between one maching and another by allowing us to define and conifgure the exact solution through the YAML file. When runing docker-compuse up, it reads that file and starts building the environment. We can also set versions within the YAML file so we can roll back to older versions if necessary. When it comes to deployment we can use that YAML file to distribute a consistent configuration, or enable an easier way of scaling an environment when necessary.  