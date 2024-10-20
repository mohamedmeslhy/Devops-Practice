# Devops-Practice
Project to apply all Devops tools

## Project: CI/CD Pipeline for a Simple Web Application
**Objective:**
To build a fully automated CI/CD pipeline for a simple web application using Docker, Jenkins, Git, a package manager, and an artifact manager.

##### Project Overview:
The project involves setting up a continuous integration and continuous deployment (CI/CD) pipeline that takes the source code from a Git repository, builds it using a package manager, stores the build artifact in an artifact manager, and deploys it into a Docker container.

##### Steps:
- Set up a Git repository:

- Create a repository (on GitHub, GitLab, or Bitbucket) to store the web application source code.
The application can be a simple web app in a language of your choice (Node.js, Python Flask, Java, etc.).

- Automate the build process with a package manager:

- Depending on the language used, set up the package manager (npm for Node.js, pip for Python, Maven for Java) to manage dependencies.
Write build scripts to compile and package the application.


- Write a Dockerfile that packages the app into a Docker container.
Ensure the container runs the application on a specified port.
Artifact storage:

- Set up an artifact manager like Nexus to store the build artifacts (for example, JAR files, Docker images).
- Configure Jenkins to push the build artifacts to the artifact manager.
Set up Jenkins for Continuous Integration (CI):

- Create a Jenkins pipeline that automatically triggers on each commit to the Git repository.
**In the pipeline at least:**
  1. Pull the latest code from the Git repository.
  2. Build the application using the package manager.
  3. Push the built artifacts to the artifact manager.
  4. Build the Docker image.
  5. Deploy the app using Docker:

- Add a deployment stage to the Jenkins pipeline, where the Docker image is pulled and deployed on a local environment.

##### Expected Outcome:
By the end of this project, you will have:

- A Git repository integrated with Jenkins for CI/CD.
- A package manager setup to build your application.
- An artifact manager storing your build artifacts.
- Docker containers running your application.
- A fully automated CI/CD pipeline with continuous integration, continuous deployment.
