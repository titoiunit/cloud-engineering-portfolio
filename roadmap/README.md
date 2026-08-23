# Cloud & DevOps Depth-Building Roadmap

This roadmap prioritizes high-signal labs that deepen operational judgment without creating unnecessary cloud spend.

## Next

| Priority | Lab | Main signal | Cost approach |
|---:|---|---|---|
| 1 | VPC gateway endpoints for S3 and DynamoDB | Private AWS access, route tables and endpoint policies | Start with gateway endpoints; avoid NAT Gateway and interface endpoints unless the scenario requires them |
| 2 | Event-driven hardening | DLQ, retry, idempotency, replay and observability | Extend the existing S3/Lambda/SQS/SNS work |
| 3 | CloudWatch operations pack | Alarm design, dashboards and incident runbook | Small scope, short retention and cleanup |
| 4 | Secrets rotation | Least privilege, secret lifecycle and rotation failure handling | One secret, timeboxed test and immediate cleanup |
| 5 | ECS blue/green deployment | Release safety, health checks and rollback | Short-lived Fargate/ALB environment only for validation |
| 6 | RDS recovery exercise | Backup, restore, RTO/RPO and failure communication | Document the design first; timebox any managed database test |
| 7 | Kubernetes foundations → EKS validation | Deployment, service, ingress and operational trade-offs | Build locally first, then run a short EKS validation only when ready |
| 8 | WAF, DNS and HTTPS edge security | Public-edge protection, ACM and Route 53 | Timeboxed test; do not leave WAF or load balancers running |

## Why this order

The first four projects improve the existing portfolio with security, operations and reliability evidence. The later projects introduce services that can produce recurring costs, so they are designed as short, deliberate validations rather than always-on demos.

## Rule for every roadmap item

It moves from **planned** to **featured** only after code, validation evidence, operational notes and cleanup instructions meet the [Portfolio Lab Standard](../lab-standards/README.md).
