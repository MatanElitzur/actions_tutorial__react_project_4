# actions_tutorial__react_project_4
actions_tutorial__react_project_4

This action project handle environment variables 

In the code for example in data\database.js
we are using environment variables like the following
const clusterAddress = process.env.MONGODB_CLUSTER_ADDRESS;
const dbUser = process.env.MONGODB_USERNAME;
const dbPassword = process.env.MONGODB_PASSWORD;
const dbName = process.env.MONGODB_DB_NAME;

We need to pass those variables from the github action workflow

# GitHub Actions also provides a couple of default environment variables that are set automatically:

https://docs.github.com/en/actions/learn-github-actions/environment-variables#default-environment-variables

# These environment variable can, for example, give you quick access to the repository to which the workflow belongs, the name of the event that triggered the workflow and many other things.