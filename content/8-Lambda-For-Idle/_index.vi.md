---
title: "Write a Lambda to Check for Idle Resources (e.g., Inactive EC2 Instances)"
date: 2024-01-01T10:00:00+07:00
weight: 8
chapter: false
pre: " <b> 8. </b> "
---

#### Step 1. Create a Lambda function: Go to AWS Management Console → Lambda → Create function.

![Error Picture](/images/AWS-Pic/CreLambdaFunc.png)

#### Step 2. Grant IAM Permissions to Lambda

> #### Step 2.1. Go to IAM → Roles → Create Roles

![Error Picture](/images/AWS-Pic/CreLambdaFunc.png)

> #### Step 2.2. Select Lambda

![Error Picture](/images/AWS-Pic/Lambda.png)

> #### Step 2.3. Attach policies

> #### - AmazonEC2ReadOnlyAccess (Allows Lambda to read EC2 information)

> #### - CloudWatchReadOnlyAccess (Allows Lambda to read metrics from CloudWatch, required to retrieve CPUUtilization data from the past 7 days)

> #### - AmazonSNSFullAccess (Allows Lambda to send notifications via SNS)

> #### - AmazonEC2FullAccess (Allows Lambda to stop EC2 instances)

![Error Picture](/images/AWS-Pic/Policy_1.png)
![Error Picture](/images/AWS-Pic/Policy_2.png)
![Error Picture](/images/AWS-Pic/Policy_3.png)
![Error Picture](/images/AWS-Pic/Policy_4.png)

> #### - Name the role: LambdaIdleEC2Policy

> #### Step 2.4. Assign the newly created role to the Lambda function

> #### - In the Lambda console, select the function you created → Configuration → Permissions → Edit

![Error Picture](/static/images/AWS-Pic/GanRoleVsLambda.png)

> #### - Select the newly created role

![Error Picture](/static/images/AWS-Pic/ChooseRole.png)

#### Step 3. Write Lambda Code (Python) (Example: Check EC2 instances with CPUUtilization < 5% in the past 7 days)

> #### - In Lambda, select the created function → go to the Code tab

![Error Picture](/static/images/AWS-Pic/TabCode.png)

> #### - Source Code

![Error Picture](/static/images/AWS-Pic/SourceCode.png)
