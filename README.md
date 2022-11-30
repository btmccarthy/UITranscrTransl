# UITranscrTransl
Repo for AWS lambda functions for Unemployment Insurance Transcribe / Translate workload / PoC

The lambda functions will each be triggered by an S3 object creation event, except for lmbda_transcribe_text
and lambda_APIGateway, which will be triggered by a transcribe job and API Gateway, respectively.

There is an additional lambda function used for dumping DynamoDB data into S3 so the data can be 
retrieved from Athena for the QuickSight dashboard. However, a CloudFormation template was used
in this case. This function / connection can be created in the console automatically when establishing
a data source connection to DynamoDB via Athena. Further instructions can be found in this article:
https://dev.to/awscommunity-asean/visualising-your-amazon-dynamodb-data-with-amazon-quicksight-14n4#step2
