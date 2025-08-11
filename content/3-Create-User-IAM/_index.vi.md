---
title: "Create Personal IAM User for Work"
date: 2024-01-01T10:00:00+07:00
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

#### Step 1. Go to IAM → User → Add User

![Error Picture](/static/images/AWS-Pic/IAM-User.png)
![Error Picture](/static/images/AWS-Pic/AddUserr.png)

#### Step 2. Create a user named “finops-user” and select "AWS Management Console access"

![Error Picture](/static/images/AWS-Pic/CreUser.png)

#### Step 3. Create “Permission sets” for the user

> #### 1. Go to Permission set

![Error Picture](/static/images/AWS-Pic/VaoPer.png)

> #### 2. Create a Permission set

![Error Picture](/static/images/AWS-Pic/TaoPer.png)

> #### 3. Select Custom permission set → Next

![Error Picture](/static/images/AWS-Pic/CusPer.png)

> #### 4. Select the following policies: “Billing”, “CostExplorerReadOnlyAccess”, “BudgetsReadOnlyAccess”, “AWSBillingReadOnlyAccess”, “ViewOnlyAccess”

![Error Picture](/static/images/AWS-Pic/Billing.png)

![Error Picture](/static/images/AWS-Pic/Access.png)

![Error Picture](/static/images/AWS-Pic/Billing-Access.png)

![Error Picture](/static/images/AWS-Pic/View-Access.png)

#### Step 5. Name the permissions “FinOpsBillingAccess” and add a description

![Error Picture](/static/images/AWS-Pic/FinOpsAccess.png)

#### Step 6. Assign the “User” to the “Permission set”

> #### 1. Go to the “AWS Account” tab → Click the User → Assign users or groups.

![Error Picture](/static/images/AWS-Pic/AssignUser.png)

> #### 2. In the Users tab, select the user to assign the Permission set → Next

![Error Picture](/static/images/AWS-Pic/TabUser.png)

> #### 3. Select the previously created Permission set → Next

![Error Picture](/static/images/AWS-Pic/SetPer.png)

> #### 4. Review

![Error Picture](/static/images/AWS-Pic/CheckPer.png)
