# actions_tutorial__react_project_4

# This action project handle environment variables & Secrets

# Docker
Using docker container and services containers 
# Secrets
https://docs.github.com/en/actions/security-guides/encrypted-secrets
After creating a a secret in github you can not see it again, but you can update it
# Secrets can be store in two places:
1. in gitgub ui in the organization account by clicking on the settings this is good when you have several repositories that uses the same secrets.
2. In a specific repository click on the repository settings, under security click on secrets then click on actions

#  environment variables
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
