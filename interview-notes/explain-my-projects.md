# Explaining My Cloud & DevOps Work

Use these short narratives to explain the portfolio clearly and honestly in interviews.

## Positioning

> I am a hands-on Cloud and DevOps-focused engineer. I build cloud infrastructure with Terraform, connect it to application delivery, and document the security, operational and cost decisions behind it. My strongest platform is AWS, and I am extending the same architecture patterns into Azure.

## 30-second introduction

> My work focuses on repeatable cloud delivery: Terraform for infrastructure, Docker for application packaging, GitHub Actions and OIDC for CI/CD, and AWS services such as ECS, Lambda, RDS, CloudWatch and VPC. I learn by building end-to-end systems, validating them, cleaning up temporary resources and documenting both the trade-offs and the operational path.

## Project stories

### 1. Terraform + GitHub Actions + AWS OIDC

**Situation:** I wanted a deployment workflow that did not depend on long-lived AWS credentials in GitHub.

**Action:** I built GitHub Actions workflows that use OIDC to assume AWS IAM roles, validate and apply Terraform, build Docker images and publish commit-SHA and environment tags to Amazon ECR.

**Result:** I gained a repeatable delivery path with short-lived credentials, remote Terraform state and traceable image versions.

**What I would improve next:** Add pull-request plans, protected environments and an explicit rollback runbook.

### 2. AWS architecture portfolio

**Situation:** I wanted to understand when to choose traditional compute, serverless or containers instead of memorizing individual AWS services.

**Action:** I built and documented multiple patterns: EC2 + RDS, API Gateway + Lambda + DynamoDB, S3-triggered processing, Auto Scaling, ECS Fargate and static delivery.

**Result:** I can explain the operational trade-offs between server management, scaling behavior, data stores, cost and security boundaries.

**What I would improve next:** Add fuller deployment evidence, monitoring and failure-testing notes to every lab.

### 3. Azure hands-on path

**Situation:** I wanted cloud knowledge that transfers across providers.

**Action:** I mapped AWS concepts to Azure and built a structured Azure path across storage, compute, serverless, containers, monitoring and Terraform.

**Result:** I can discuss the architecture concept first, then the provider-specific service choice.

## Answer pattern for architecture questions

```text
1. Start with the workload or business need
2. Name the constraints: security, availability, operations and cost
3. Explain the chosen architecture
4. Mention one realistic trade-off or alternative
5. Explain how you would validate and operate it
```

## Example trade-off answers

| Question | Concise answer |
|---|---|
| ECS/Fargate or EC2? | I prefer Fargate when the team benefits from managed container infrastructure and has no need to operate hosts. EC2 gives more control but adds patching and capacity-management responsibility. |
| Lambda or a container service? | Lambda fits event-driven, short-lived workloads. A container service is a better fit for long-running processes, custom runtimes or predictable service behavior. |
| DynamoDB or RDS? | DynamoDB suits access patterns that need managed horizontal scale. RDS is the better fit for relational data, SQL queries and transactions. |
| How do you reduce cloud risk? | Least-privilege IAM, private network paths where appropriate, centralized logs and alarms, tested recovery steps, tagged resources and a documented cleanup or lifecycle plan. |

## Current depth-building areas

- ECS blue/green deployment and rollback
- RDS recovery, RTO/RPO and Multi-AZ design
- VPC endpoints and private service access
- CloudWatch monitoring and operations runbooks
- Secrets rotation
- Kubernetes foundations and cost-controlled EKS validation
- Backup and recovery testing

## Important principle

Never present a planned control as finished. State what was implemented, what was validated, and what you would add for a production workload. That makes the portfolio more credible, not less.
