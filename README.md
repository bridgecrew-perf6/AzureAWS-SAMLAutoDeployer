# AzureAWS_SAMLAutoDeployer
CloudFormation stack that deploys Azure SAML provider and adds assume role policy document to each Role in AWS Account

**Make sure to mark 'IAM capabilities'**

What it does:
1. Creates SAML provider
2. Creates IAM Role for Lambda 'Assume-Role'
3. Creates Lambda
4. Execute Lambda (send response to CloudWatch)
5. lambda mods assume-role policy document in each AWS role
6. Lambda sends response to EventBridge (CloudWatch)
