# CD12352 - Infrastructure as Code Project Solution
# [HungND]

## Spin up instructions
aws cloudformation create-stack --stack-name Network --template-body file://network.yml --parameters file://network-parameters.json
aws cloudformation create-stack --stack-name Udagram --template-body file://udagram.yml --parameters file://udagram-parameters.json --capabilities CAPABILITY_NAMED_IAM
## Tear down instructions
aws cloudformation delete-stack --stack-name Udagram
aws cloudformation delete-stack --stack-name Network
## Other considerations
TODO (optional)

URL: http://applicationloadbalancer-519049582.us-east-1.elb.amazonaws.com/