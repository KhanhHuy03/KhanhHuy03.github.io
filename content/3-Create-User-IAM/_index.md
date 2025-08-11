---
title: "Tạo User IAM Cá Nhân Để Làm Việc"
date: 2024-01-01T10:00:00+07:00
weight: 3
chapter: false
pre: " <b> 3. </b> "
---

#### Bước 1. Vào IAM → User → Add User

![Error Picture](/static/images/AWS-Pic/IAM-User.png)
![Error Picture](/static/images/AWS-Pic/AddUserr.png)

#### Bước 2. Tạo User Tên: “finops-user” và "AWS Management Console access"

![Error Picture](/static/images/AWS-Pic/CreUser.png)

#### Bước 3. Tạo “Permission sets” cho user

> #### B1. Vào Permission set

![Error Picture](/static/images/AWS-Pic/VaoPer.png)

> #### B2. Tạo Permission set

![Error Picture](/static/images/AWS-Pic/TaoPer.png)

> #### B3. Chọn Custom permission set → Next

![Error Picture](/static/images/AWS-Pic/CusPer.png)

> #### B4. Chọn các policy “Billing”, “CostExplorerReadOnlyAccess”, “BudgetsReadOnlyAccess”, “AWSBillingReadOnlyAccess”, “ViewOnlyAccess”

![Error Picture](/static/images/AWS-Pic/Billing.png)

![Error Picture](/static/images/AWS-Pic/Access.png)

![Error Picture](/static/images/AWS-Pic/Billing-Access.png)

![Error Picture](/static/images/AWS-Pic/View-Access.png)

#### Bước 5. Đặt tên permissions “”FinOpsBillingAccess” và mô tả

![Error Picture](/static/images/AWS-Pic/FinOpsAccess.png)

#### Bước 6. Gán “User” với “Permission set”

> #### B1. Vào tab “AWS Account” → Click chọn User → Assign users or groups.

![Error Picture](/static/images/AWS-Pic/AssignUser.png)

> #### B2. Trong tab Users click chọn User cần gán Permission set → Next

![Error Picture](/static/images/AWS-Pic/TabUser.png)

> #### B3. Click chọn Permission set đã tạo trước đó → Next

![Error Picture](/static/images/AWS-Pic/SetPer.png)

> #### B4. Kiểm tra kĩ → Submit

![Error Picture](/static/images/AWS-Pic/CheckPer.png)
