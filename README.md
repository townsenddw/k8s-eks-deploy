# k8s-eks-deploy
k8s on EKS deployment

# On Boarding

## Accounts and Roles

- Root Account
  - email for root account
  - Disable Key Access
- Admins: (administrator access)
  - Brian
  - Zach
  - Dwight

## EKS

- Deploy VPC
  ```bash
  aws cloudformation create-stack --stack-name eksTest --template-body file://cluster.yml --capabilities CAPABILITY_NAMED_IAM
  ```
- Deploy NodeGroup
- Set up aws-iam-authenticator (for OS X)
```
curl -o /usr/local/bin/aws-iam-authenticator https://amazon-eks.s3-us-west-2.amazonaws.com/1.10.3/2018-07-26/bin/darwin/amd64/aws-iam-authenticator
chmod +x /usr/local/bin/aws-iam-authenticator
```