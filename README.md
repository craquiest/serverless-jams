# SERVERLESS JAMS - Vote for your favorite song

## A serverless site with front and backend built with serverless framework.

Following [Serverless for Frontend Developers](https://www.serverless.com/learn/courses/serverless-for-frontend-developers/) by Fernando Medina Corey on [Serverless Learn](serverless.com/learn).

## Features 
- Authentication and Authorization with Auth0
- Static website deployment to AWS S3 with serverless-finch
- API gateway endpoints protected with Auth0 to trigger AWS Lambda functions
- API Scopes and Lambda Authorizers
- Python backend with AWS DynamoDB table to store data. 
- Nice tunes!

## Usage 
- You need to node, npm, serverless, python on your machine
- Files with data to be filled in: 
    * `serverless.yml`: fill in your app, org, AWS region, domain name (*). 
    * `frontend/auth_config.json`: fill in your Auth0 details 
    * `frontend/js/app.js`: fill in your API Gateway endpoints after 1st deployment (they appear as terminal output of your first deployment, or in your AWS console).


(*) : In order to use own domain and AWS Cloudfront, you need a separate setup either manually with AWS console or  alternatively using [Webotron](https://github.com/craquiest/aws-python-automation) in CLI. 