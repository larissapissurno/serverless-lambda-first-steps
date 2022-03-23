# serverless-lambda-first-steps

This is a POC to try the serverless framework.

The goal is:

1. Create a `index.js` file with a simple function within it;
2. Configurate a `yaml` file mapping the provider and the lambda function that was created;
3. Deploy the lambda function using the Serverless framework;

## Prerequisites

1. Make sure that you have a AWS account and [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html) configured as well.

2. Make sure you have installed all of the following prerequisites on your development machine:
   - Git;
   - Node.js and the npm package manager;
   - Serverless framework; `npm i -g serverless`

## Installing the dependencies

Once the repo is properly cloned/forked into your machine, open the terminal on the project root and run:

`npm install`

## Deploying the lambda using Serverless framework

`sls deploy --verbose`

By running this command, we can see at the logs that:

- the serverless framework will automagically create a S3 Bucket on AWS
- upload a CloudFormation file to S3
- deploy service to stack 'sls-my-first-lambda-dev'
