# UITranscrTransl
Repo for AWS lambda functions for Unemployment Insurance Transcribe / Translate workload / PoC

The lambda functions will each be triggered by an S3 object creation event, except for lmbda_transcribe_text,
dyanamocatalog, and lambda_APIGateway, which will be triggered by a transcribe job, CloudFormation, and
API Gateway, respectively.
