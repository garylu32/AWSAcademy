## Module 4
### Section 1: AWS Shared Reponsibility Model

* Customers are responsible for data security
* Security of teh cloud: physical security of data centers, hardware and software infrastructure, network infrastructure, and virtualization infrastructure

### Section 2: Identity and Access Management (IAM)

* Use IAM to mangage access to AWS resources (ex: control who can terminate Amazon EC2 instances)
* IAM is a no-cost AWS account feature
* Essential components:
  * IAM user: A person or application that can authenticate with an AWS account
  * IAM group: A collection of IAM users that are granted identical authorizaiton
  * IAM policy: The document that defines which resources can be accessed and the level of access to each resource
  * IAM role: Useful mechanism to grant a set of permissions for making AWS service requests

* Types of access the user is permitted to use:
  * Programmatic access
  * AWS Management Console access

* IAM policy is a document that defines permission
* An implict deny: is the permission explicitly denied? No ---> Is the permission explicitly allowed? Yes ---> Allow

### Section 3: Securing a new AWS account

* AWS account root user access vs. IAM access
* Best practice: Do not use the AWS account root user except when necessary
* Securing a new AWS account: Account root user
  * Step 1: stop using the account root user as soon as possible (create an IAM user for yourself)
  * Step 2: Enable multi-factor authentication (MFA)
  * Step 3: Use AWS CloudTrail, tracking activiy on your account
  * Step 4: Enable a billing report, such as AWS cost and usage report

### Section 4: Securing Accounts

* AWS organizations enables you to consolidate multiple AWS accounts so that you centrally manage them
* Amazon Cognito
* AWS shield, minimize application downtime and latency

### Section 5: Securing Data

* Encryption of data at rest, encoding data with a secret key and AWS KMS can manage your secret keys
* Encryption of data in transit, secure HTTP (HTTPS) creates a secure tunnel
* Securing Amazon S3 buckets and objects

### Section 6: Working to ensure compliance
* AWS Config: access, audit and evaluate the configuration of AWS resources
* AWS Artifact: a resouce for compliance-related inforamtion, provide access to security and compliance reports, and select online agreements
