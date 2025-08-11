---
title: "Setting up an AWS account"
date: 2024-01-01T10:00:00+07:00
weight: 1
chapter: false
---

#### Tổng quan

Trong bài thực hành đầu tiên này, bạn sẽ tiến hành tạo mới một tài khoản **AWS** và thiết lập xác thực đa yếu tố (**MFA**) để tăng cường bảo mật cho tài khoản. Tiếp theo, bạn sẽ tạo **Nhóm Quản trị viên** và **Người dùng Quản trị** nhằm quản lý quyền truy cập tài nguyên thay vì sử dụng tài khoản root.  
Cuối cùng, bạn sẽ được hướng dẫn xác thực tài khoản với **AWS Support** trong trường hợp gặp sự cố về đăng nhập

#### FinOps Implementation with Automated Cost Governance trên AWS

FinOps là phương pháp kết hợp giữa tài chính và vận hành nhằm tối ưu hóa chi phí điện toán đám mây một cách chủ động và minh bạch. Trên AWS, việc triển khai FinOps với các công cụ tự động giúp doanh nghiệp kiểm soát, dự báo và tối ưu hóa chi tiêu hiệu quả hơn. Bằng cách tích hợp các giải pháp như AWS Budgets, Cost Anomaly Detection, Cost & Usage Report, Compute Optimizer và tự động hóa kiểm tra tài nguyên không sử dụng, tổ chức có thể phát hiện sớm các bất thường về chi phí, chủ động xử lý và liên tục cải tiến chính sách quản trị chi phí. Điều này không chỉ giúp tiết kiệm ngân sách mà còn nâng cao hiệu quả sử dụng tài nguyên AWS, đảm bảo phù hợp với mục tiêu kinh doanh và phát triển bền vững trên nền tảng đám

#### Main Content

1. [Giới thiệu đề tài](1-introduce/)
2. [Bật Billing Access](2-billing-access)
3. [Tạo User IAM Cá Nhân Để Làm Việc](3-create-user-iam/)
4. [Tạo AWS Budget](4-create-aws-budget/)
5. [Tạo AWS Cost Anomaly](5-create-aWS-cost-anomaly-detection/)
6. [Bật Cost & Usage Report (CUR)](6-cost-&-usage-report/)
7. [Bật AWS Compute Optimizer](7-aWS-compute-optimizer/)
8. [Viết lambda kiểm tra tài nguyên idle (VD: EC2 không hoạt động)](8-lambda-for-idle/)
9. [Tạo CloudWatch Dashboard](10-create_cloudwatch-dashboard/)
10. [Viết SOP Xử Lý Chi Phí Vượt Ngân Sách](11-sopp/)

<!-- 9. [Gửi Log vào S3 hoặc SNS](\9-log-in-s3-or-sns/) -->
