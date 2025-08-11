---
title: " Viết Lambda kiểm tra tài nguyên idle (VD: EC2 không hoạt động)"
date: 2024-01-01T10:00:00+07:00
weight: 8
chapter: false
pre: " <b> 8. </b> "
---

#### Bước 1. Tạo Lambda function: Vào AWS Management Console → Lambda → Create function.

![Error Picture](/static/images/AWS-Pic/CreLambdaFunc.png)

#### Bước 2. Cấp quyền IAM cho Lambda

> #### B1. Vào IAM → Roles → Create Roles

![Error Picture](/static/images/AWS-Pic/CreLambdaFunc.png)

> #### B2. Chọn Lambda

![Error Picture](/static/images/AWS-Pic/Lambda.png)

> #### B3. Gán policy

> #### - AmazonEC2ReadOnlyAccess (Cho phép Lambda đọc thông tin EC2 ),

> #### - CloudWatchReadOnlyAccess (Cho phép Lambda đọc metrics từ CloudWatch, Cần để lấy dữ liệu CPUUtilization 7 ngày qua),

> #### - AmazonSNSFullAccess (Cho phép Lambda gửi thông báo qua SNS),

> #### - AmazonEC2FullAccess(dừng EC2)

![Error Picture](/static/images/AWS-Pic/Policy_1.png)
![Error Picture](/static/images/AWS-Pic/Policy_2.png)
![Error Picture](/static/images/AWS-Pic/Policy_3.png)
![Error Picture](/static/images/AWS-Pic/Policy_4.png)

> #### - Đặt tên role: LambdaIdleEC2Policy

> #### B4. Gán Lambda vừa tạo cho Role “LambdaIdleEC2Policy”,

> #### - Trong màn hình Lambda chọn funtion đã tạo → Configuration → Permissions → Edit

![Error Picture](/static/images/AWS-Pic/GanRoleVsLambda.png)

> #### - Chọn role vừa mới tạo

![Error Picture](/static/images/AWS-Pic/ChooseRole.png)

#### Bước 3. Code Lambda (Python) (Ví dụ kiểm tra EC2 có CPUUtilization < 5% trong 7 ngày qua)

> #### - Trong Lambda chọn function đã tạo → tab code

![Error Picture](/static/images/AWS-Pic/TabCode.png)

> #### - Source Code

![Error Picture](/static/images/AWS-Pic/SourceCode.png)
