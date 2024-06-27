## Project Management with Docker and CI/CD

13. **Describe the role of GitHub Actions in your project's CI/CD pipeline. How do you automate testing and deployment using GitHub Actions?**

The way that the project utilizes GitHub Actions is through the use of workflow definitials. For example, in the project we are utilizing the production.yml file under the .github/workflows folder. Within our project settings in GitHub we identify the workflow we will be using, in this case "production" and an github picks up our production YAML file and starts to execture its config.
Within the YAML file, we specify which action automatically triggers its execution and then which jobs and steps to run. We can include multiple jobs that can either run one after another, or nest them so they are reliant on the success of a previously run jobs.