# DRAFT - A Step-by-Step Guide - Calling the Jurassic-2 (J2) Large Language Model through an AWS Lambda Endpoint

## Purpose of this guide

This guide was created as a companion for the blog [This is a placeholder link -> [How to access the Jurassic-2 (J2) large language model via an AWS Lambda endpoint]](https://aws.amazon.com/blogs/apn/). The deployment guide will walk you through all the needed steps to deploy the solution referred to in the blog post.

## Prerequisites

This section will cover any prereqs. needed to run the solution.

### AI21 Labs account

In order to use the Jurassic-2 model you will need an API key from AI21 Labs.

1. [Sign up for a free account](https://www.ai21.com/studio/pricing)
2. [Access your API key here](https://studio.ai21.com/account/api-key)

You will need your AI21 Labs API key in Step 2 when deploying your CloudFormation template.

#### Note: Click the link for each step to go through the deployment guide.

## [Step 1 - Deploying AWS Lambda layer](./docs/layer.md)

This section we will walk you through all the steps needed to deploy the lambda layer needed for the lambda function to include the AI21 Lab's Python SDK library. This library is needed for the lambda function to communicate with the Jurassic-2 model.

## [Step 2 - Deploying CloudFormation template](./docs/cfn.md)

This section will walk you through how to deploy the CloudFormation template for the solution. The CloudFormation template will spin up all the needed resources for you to run this solution in a demo environment.

## [Step 3 - Adding layer to lambda endpoint](./docs/adding_layer.md)

This section will walk you through how to add the lambda layer you created in step 1 to the lambda function that was created when you deployed the CloudFormation template in step 2.

## [Step 4 - Testing](./docs/test.md)

This section will walk you through how to test the lambda endpoint that will return results from the Jurassic-2 LLM.

## [Step 5 - Cleanup](./docs/cleanup.md)

This section cover how to remove all AWS resources that were created when we deployed the CloudFormation template.
