---
title: "Giới thiệu"
date: 2024-01-01T10:00:00+07:00
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

#### Giới thiệu

Trong bối cảnh chuyển đổi số mạnh mẽ, việc sử dụng dịch vụ điện toán đám mây như AWS ngày càng phổ biến nhằm tối ưu hóa hạ tầng công nghệ thông tin và nâng cao hiệu quả vận hành. Tuy nhiên, đi kèm với sự linh hoạt và mở rộng của đám mây là thách thức trong việc kiểm soát và tối ưu chi phí. Đề tài "FinOps Implementation with Automated Cost Governance trên AWS" tập trung vào việc áp dụng các phương pháp quản trị tài chính hiện đại (FinOps) kết hợp với các công cụ tự động hóa của AWS để giúp doanh nghiệp chủ động giám sát, phát hiện bất thường và tối ưu hóa chi tiêu trên nền tảng đám mây. Qua đó, tổ chức có thể đảm bảo sử dụng tài nguyên hiệu quả, tiết kiệm ngân sách và hỗ trợ mục tiêu phát triển bền

#### Kiến trúc giải pháp và các dịch vụ sử dụng

Giải pháp FinOps với Automated Cost Governance trên AWS được xây dựng dựa trên kiến trúc tích hợp nhiều dịch vụ AWS nhằm tự động hóa việc giám sát, phân tích và tối ưu hóa chi phí. Kiến trúc này bao gồm các thành phần chính như sau:

- **AWS Budgets**: Thiết lập ngân sách, theo dõi chi tiêu và gửi cảnh báo khi vượt ngưỡng.
- **AWS Cost Anomaly Detection**: Tự động phát hiện các bất thường về chi phí và cảnh báo kịp thời.
- **AWS Cost & Usage Report (CUR)**: Thu thập và phân tích chi tiết dữ liệu sử dụng và chi phí.
- **AWS Compute Optimizer**: Đưa ra khuyến nghị tối ưu hóa tài nguyên tính toán như EC2, EBS, Lambda.
- **AWS Lambda**: Tự động kiểm tra và xử lý các tài nguyên không sử dụng hoặc hoạt động kém hiệu quả.
- **Amazon CloudWatch**: Giám sát, thu thập log và trực quan hóa dữ liệu chi phí, hiệu suất.
- **Amazon SNS (Simple Notification Service)**: Gửi thông báo tự động đến email, Slack hoặc các kênh liên lạc khác.
- **Amazon S3**: Lưu trữ báo cáo, log và dữ liệu phân tích chi phí.

Các dịch vụ này phối hợp với nhau tạo thành một hệ thống quản trị chi phí tự động, giúp doanh nghiệp chủ động kiểm soát, phát hiện sớm các vấn đề và tối ưu hóa chi tiêu trên AWS một cách hiệu quả và minh
