
Jenkins Pipeline with Docker and Node.js
This README provides an overview of the Jenkins pipeline configured for a project using Node.js with Docker. The pipeline automates the build and test process within a Docker container running Node.js version 14.

Pipeline Overview
The pipeline is defined in a declarative syntax and consists of the following components:

Agent
The pipeline uses the Node.js 14 Docker image (node:14) to ensure consistency across environments.
Stages
Checkout
Pulls the code from the repository configured in Jenkins (checkout scm).
Build
Verifies the installed Node.js version within the Docker container (node --version).
Test
Placeholder stage for running tests (echo "Running tests...").
Post Conditions
Success
Displays a message: "Build and Test succeeded!"
Failure
Displays a message: "Build or Test failed!"
Prerequisites
Before running this pipeline, ensure the following:

Jenkins Setup:

Jenkins is installed and running.
Docker plugin for Jenkins is installed.
Git Repository:

The pipeline is connected to a valid Git repository.
The scm in the pipeline points to your repository.
Docker:

Docker is installed on the Jenkins server or agent.
Jenkins has permissions to run Docker commands.
