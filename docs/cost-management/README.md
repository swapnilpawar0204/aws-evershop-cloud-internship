# AWS cost management & cleanup checklist

AWS billing depends on account eligibility, region, usage, and current pricing. Confirm pricing and Free Tier/credits eligibility before creating resources.


## Before starting
- [ ] Set a budget alert and review billing dashboard/Cost Explorer.
- [ ] Confirm region and avoid unnecessary multi-region resources.
- [ ] Prefer local Docker or diagrams for learning when a live AWS deployment is not required.
- [ ] Understand whether each resource incurs hourly, storage, request, data-transfer, or other charges.
- [ ] Use short sessions; record resources created and their names/tags.

## Cleanup inventory (check all regions)
- [ ] EC2 instances stopped or terminated as intended (stopping may still leave charges for storage or other resources)
- [ ] EBS volumes and snapshots reviewed; delete only if no longer needed
- [ ] Elastic IP addresses released when unused
- [ ] Load balancers deleted if no longer needed
- [ ] NAT Gateways removed if not needed (can be costly)
- [ ] RDS instances deleted or stopped where supported; snapshots reviewed
- [ ] ECS services/tasks/clusters reviewed and removed if no longer required
- [ ] ECR images/repositories reviewed for storage
- [ ] S3 buckets emptied and removed if no longer required
- [ ] CloudFront distributions disabled/deleted where appropriate
- [ ] Route 53 hosted zones/records reviewed; hosted zones may incur charges
- [ ] CloudWatch log groups, alarms, dashboards, and retained logs reviewed
- [ ] Certificate resources and other services reviewed for applicable charges
- [ ] Check AWS Billing/Cost Explorer after cleanup for residual costs

> Never delete a resource until you understand whether it contains data you need. AWS cleanup is not complete until you review all regions and billing.
