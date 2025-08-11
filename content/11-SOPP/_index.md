---
title: "SOP Xử Lý Chi Phí Khi Vượt Ngân Sách"
date: 2024-01-01T10:00:00+07:00
weight: 10
chapter: false
pre: " <b> 10. </b> "
---

#### B1. Phát hiện

- AWS Budgets hoặc Cost Anomaly Detection gửi cảnh báo qua Email, Slack hoặc SNS.

#### B2. Xác nhận

- Kiểm tra số liệu thực tế trên AWS Cost Explorer hoặc Billing Dashboard.

#### B3. Phân tích nguyên nhân

- Xác định dịch vụ nào tăng chi phí (ví dụ: EC2, S3, RDS…).
- Phân loại nguyên nhân: có thể kiểm soát / không thể kiểm soát.

#### B4. Hành động

- Giảm hoặc tắt các tài nguyên không cần thiết (EC2, Auto Scaling, unused volumes).
- Hoặc xin phê duyệt tăng ngân sách nếu thực sự cần thiết.

#### B5. Ghi nhận & cập nhật

- Lưu lại báo cáo về nguyên nhân và các hành động đã thực hiện.
- Điều chỉnh policy hoặc automation rule để tránh lặp lại sự cố tương tự.
