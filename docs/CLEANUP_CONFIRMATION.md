# Clean-Up Confirmation

**Project:** Modernizing and Optimizing Infrastructure for AI Workloads and Solutions  
**Course:** AWS Serverless Cloud Architecture  
**Company Case Study:** ObjectionInspection Inc.  
**AWS Region:** us-east-1  
**AWS Account ID:** 117913377161  
**Stack Name:** test-stack  

---

## Clean-Up Statement

I confirm that I have deleted and cleaned up all AWS resources created during the testing, deployment, and verification of this solution, including:

1. **Amazon S3 Buckets & Objects:**
   - Emptied all objects, versions, and delete markers from input bucket: `objection-inspection-input-117913377161-us-east-1`
   - Emptied all objects, versions, and delete markers from output bucket: `objection-inspection-output-117913377161-us-east-1`
   - Deleted both S3 buckets.

2. **AWS Lambda:**
   - Deleted function `objection-inspection-summarizer` and its associated versions and aliases.

3. **AWS IAM:**
   - Deleted IAM execution role `objection-inspection-lambda-execution-role-us-east-1` and all attached inline policies (`CloudWatchLogsPolicy`, `S3AccessPolicy`, `BedrockInvokePolicy`).
   - Removed resource-based Lambda invocation permission (`LambdaInvokePermission`).

4. **Amazon CloudWatch:**
   - Deleted log group `/aws/lambda/objection-inspection-summarizer` and log streams.

5. **AWS CloudFormation:**
   - Deleted CloudFormation stack `test-stack`.
   - Verified `DELETE_COMPLETE` status via AWS CLI.

---

**Confirmation Statement:**  
*I confirm that all AWS resources (buckets, Lambda functions, IAM roles, and CloudFormation stacks) created for testing this project have been fully deleted and cleaned up after testing.*

**Signed:** Senior AWS Solutions Architect  
**Date:** October 17, 2026
