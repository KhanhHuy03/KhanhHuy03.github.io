---
title: "Tạo CloudWatch Dashboard"
date: 2024-01-01T10:00:00+07:00
weight: 9
chapter: false
pre: " <b> 9. </b> "
---

#### Bước 1. Vào AWS Console → CloudWatch → Dashboards → Create dashboard.

![Error Picture](/static/images/AWS-Pic/DashBoard.png)

#### Tên Dashboard vd: FinOps-Cost-Dashboard

#### Bước 2. Chọn loại widget

![Error Picture](/static/images/AWS-Pic/Widget.png)

#### Bước 3. Bật AWS/Billing metric để dùng trong Dashboard FinOps

> #### - Vào Billing → Trong menu trái → Billing preferences → Edit

![Error Picture](/static/images/AWS-Pic/BillingPreference.png)

> #### - Tick chọn Receive Billing Alerts → Save.

![Error Picture](/static/images/AWS-Pic/AlertPre.png)

#### Bước 4. Quay lại CloudWatch, Chọn Metrics → bạn sẽ thấy namespace AWS/Billing xuất hiện.

#### Bước 5. Thêm widget

> #### Quay lại Dashboard → Add widget.

> #### Browse → chọn AWS/Billing.

> #### Thêm metric EstimatedCharges → chọn loại hiển thị (Line, Number…) → Create
