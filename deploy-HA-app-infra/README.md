# Deploy HA webapp using CloudFormation
The below is built for aws solution using cloudformation templates. This built upon fundamentals of assuming your infrastructure is destructible. I've deployed sample dockerized container with Tomcat webserver into ec2, but this can be extended  to CD/CI setup.

## setup
1. `Install awscli and configure`
2. `Update outinfra-parameters.json with custom parameters.`
3. `demoservers.json with custom parameters.`

## Usage
### Usage cloudformation create stack
```
aws cloudformation create-stack --stack-name <stack name> --template-body outinfra.yml --parameters file://outinfra-params.json


aws cloudformation create-stack --stack-name <stack name> --template-body demoservers.yml --parameters file://demoservers.json
```
### Usage cloudformation update stack for re-runs
```
aws cloudformation update-stack --stack-name <stack name> --template-body outinfra.yml --parameters file://outinfra-params.json


aws cloudformation update-stack --stack-name <stack name> --template-body demoservers.yml --parameters file://demoservers.json
```



