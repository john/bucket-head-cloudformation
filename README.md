# bucket-head-cloudformation

## Manual steps:

- Update the Elastic Transcoder pipeline to pull from and write to the most recently created S3 buckets.
- Make sure the API Gateway methods are pulling from the most recent DynamoDB table.
- Lambda to update DynamoDB needs to be able to get most recent table for transcoded files, instead of hardcoding

### ToDo
Have CF create the secondary index on the videos table.

Services used:

CloudFormation
S3
Lamba
ElasticTranscoder
SNS
DynamoDB
API Gateway
Cognito

Soon:
Transfer Acceleration
CloudFront (for client, can put in front of Fryolator)