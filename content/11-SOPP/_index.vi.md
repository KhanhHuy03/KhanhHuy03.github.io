---
title: "SOP for Handling Costs When Budget is Exceeded"
date: 2024-01-01T10:00:00+07:00
weight: 10
chapter: false
pre: " <b> 10. </b> "
---

#### Step 1. Detection

- AWS Budgets or Cost Anomaly Detection sends alerts via Email, Slack, or SNS.

#### Step 2. Verification

- Check the actual figures in AWS Cost Explorer or the Billing Dashboard.

#### Step 3. Root Cause Analysis

- Identify which service has increased costs (e.g., EC2, S3, RDS…).
- Classify the cause: controllable / uncontrollable.

#### Step 4. Action

- Reduce or shut down unnecessary resources (EC2, Auto Scaling, unused volumes).
- Or request approval to increase the budget if genuinely necessary.

#### Step 5. Documentation & Update

- Record the report detailing the cause and actions taken.
- Adjust policies or automation rules to prevent similar incidents in the future.
