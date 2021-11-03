# aws-lambda-function-template

A template repository to get started with developing AWS Lambda functions

- Package and push to ECR (Elastic Container Registry)
- Deploy to AWS Lambda functions (Not through CloudFormation)

> Both the **Build** and **Deploy** steps in the pipeline steps are CodeBuild projects having specs `buildspec.yml` and `deployspec.yml` respectively

## Enviornment Variables

### Build

- `AWS_DEFAULT_REGION`
- `AWS_ACCOUNT_ID`
- `IMAGE_REPO_NAME` - The ECR repository name
- `IMAGE_TAG` - Image tag to be deployed (`latest`)

### Deploy

- `IMAGE_URI`
- `LAMBDA_FUNCTION_NAME`

> _`function/scripts`_ contains shell scripts for easy deployments without the pipeline setup!
