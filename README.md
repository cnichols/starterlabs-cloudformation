# starterlabs-cloudformation
Starter Labs Cloud Formation


### CommonVPC
aws cloudformation create-stack \
  --stack-name common-vpc \
  --template-body file://common/templates/vpc.yml \
  --parameters file://common/parameters/vpc-parameters.json \
  --capabilities CAPABILITY_NAMED_IAM \
  --region us-east-1

### CommonSecurityGroups
aws cloudformation create-stack \
  --stack-name common-security-groups \
  --template-body file://common/templates/security-groups.yml \
  --capabilities CAPABILITY_NAMED_IAM \
  --region us-east-1