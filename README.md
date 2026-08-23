# Cloud & DevOps Engineering Portfolio

Hands-on portfolio of AWS, Azure, Terraform, Docker, Python and CI/CD work.

I build cloud solutions with a practical engineering mindset: clarify the operational need, choose the simplest secure architecture that meets it, automate it with Infrastructure as Code, validate the result, and document the trade-offs and cleanup.

## What I bring

- **Infrastructure as Code:** Terraform modules, environment structure, remote state and repeatable deployments
- **AWS architecture:** VPC networking, EC2, RDS, S3, CloudFront, API Gateway, Lambda, DynamoDB, SQS/SNS, ECS Fargate and Auto Scaling
- **DevOps delivery:** Dockerized workloads, GitHub Actions, OIDC-based AWS authentication, deployment and rollback thinking
- **Cloud operations:** CloudWatch, logging, alarms, cost awareness, least-privilege IAM and cleanup discipline
- **Application context:** Python services, PostgreSQL and API fundamentals

## Featured work

| Project | Architecture / focus | What it demonstrates |
|---|---|---|
| [AWS Infrastructure Architectures](https://github.com/titoiunit/aws-infrastructure-architectures) | EC2 + RDS, serverless API, event-driven processing, Auto Scaling, ECS Fargate and static delivery | Choosing compute patterns, Terraform, networking, security boundaries and scalable design |
| [AWS Terraform Infrastructure](https://github.com/titoiunit/aws-terraform-infrastructure) | Terraform, remote state, Docker, GitHub Actions OIDC and Amazon ECR delivery | Reusable IaC, environment separation, short-lived cloud credentials and repeatable delivery |
| [Azure Hands-on Projects](https://github.com/titoiunit/azure-hands-on-projects) | Storage, Linux VM, Functions, event-driven processing, containers, monitoring and Terraform | Transferable cloud concepts across AWS and Azure |
| [Python Production Backend Template](https://github.com/titoiunit/python-production-backend-template) | Python service foundations, configuration and structured logging | How application behavior, operations and cloud deployment connect |

## Engineering approach

```text
Understand the workload
→ assess security, availability and cost constraints
→ design the smallest appropriate architecture
→ implement with Terraform and version control
→ validate deployment and failure paths
→ add observability and document operations
→ clean up temporary resources
```

A working deployment alone is not the finish line; the project must also be explainable, maintainable and cost-conscious.

## Evidence standards

Each completed project is documented against the same standard:

1. **Problem and constraints** — what the workload needed and what was deliberately out of scope  
2. **Architecture and decisions** — services used, alternatives considered and key trade-offs  
3. **Implementation** — Terraform, application or automation components  
4. **Security and operations** — IAM, network boundaries, logging, alarms and failure handling  
5. **Validation** — how the deployment and important paths were tested  
6. **Cost and cleanup** — guardrails, resources to destroy and proof of safe teardown  
7. **Interview summary** — a concise explanation of the business value and engineering choices  

## Current depth-building roadmap

- ECS blue/green deployments and rollback validation
- RDS recovery, RTO/RPO and Multi-AZ trade-offs
- Private AWS access with VPC endpoints
- CloudWatch monitoring, alarms and operational runbooks
- Secrets rotation and least-privilege access
- Kubernetes foundations, then a cost-controlled EKS validation
- Backup and recovery testing

## Repository map

- `architecture-maps/` — cross-cloud and service-pattern comparisons
- `case-studies/` — deeper explanations of completed work
- `interview-notes/` — concise, evidence-based interview narratives

## Status

Active portfolio. I build the implementation first, then publish the architecture, validation evidence and operational notes that support it.
