# DevOps Challenge

I made this Repository for the DevOps Challenge.

## Requirements

- AWS CLI
- AWS Credentials
- EC2-Keypair

## Use

You can use this Command to create the stack

aws cloudformation create-stack --stack-name $stackname --template-body file://templates/Webserver.yaml --parameters ParameterKey=ParameterKeyName,ParameterValue=webserver-keykeypair

Note:
- Make sure you replace the parameter value with your aws keypair name!
- Pick the stackname

## Deletion

aws cloudformation delete  --stack-name $stackname

You can use this command to delete the stack

## Next Step :
- Add Loadbalancer to the Cloudformation
- Add HTTPS endpoints instead of http
- Add CloudFront
- Add ASG to the stack to provide scaling and better availability
