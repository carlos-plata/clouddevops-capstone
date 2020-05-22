[![CircleCI](https://circleci.com/gh/carlos-plata/clouddevops-capstone.svg?style=svg)](https://circleci.com/gh/carlos-plata/clouddevops-capstone)


# Udacity Nanoedegree - Cloud DevOps Engineer - Capstone project

Uses AWS Cloudformation Template as base template. https://github.com/aws-samples/ecs-refarch-cloudformation


Builds the infrastructure using AWS CloudFormation


Uses AWS S3 to store builds and cloudformation templates


Builds java app with Maven.


Applies PMD code analysis with Maven PMD plugin.


Runs unit tests with Maven.


Builds Docker image with Maven plugin.


Deploys a Websocket Java Webchat app to AWS with CircleCI.


Rolls out a Blue/Green deployment based on cloudformation configuration in services.yml:


DesiredCount: 2


DeploymentConfiguration:

    MaximumPercent: 100
    MinimumHealthyPercent: 50

    
The previous configuration allows to have a 100% of the available tasks (2) running, while maintaining 50% (1) of the available tasks handling the load during a deploy.
