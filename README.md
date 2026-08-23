# Cloud & DevOps Engineering Portfolio

Hands-on portfolio of AWS, Azure, Terraform, Docker, Python, and CI/CD work.

I build cloud solutions with a practical engineering mindset: clarify the operational need, choose the simplest secure architecture that meets it, automate it with Infrastructure as Code, validate the result, and document the trade-offs and cleanup.

## What I bring

- **Infrastructure as Code:** Terraform modules, environment structure, remote state, and repeatable deployments.
- **AWS architecture:** VPC networking, EC2, RDS, S3, CloudFront, API Gateway, Lambda, DynamoDB, SQS, ECS Fargate, and Auto Scaling.
- **DevOps delivery:** Dockerized workloads, GitHub Actions, OIDC-based AWS authentication, deployment, and rollback thinking.
- **Cloud operations:** CloudWatch, logging, alarms, cost awareness, least-privilege IAM, and cleanup discipline.
- **Application context:** Python, PostgreSQL, and API fundamentals — enough to collaborate effectively with application teams.

## Implemented work

| Project | Architecture / focus | What it demonstrates |
|---|---|---|
| [AWS Infrastructure Architectures](https://github.com/titoiunit/aws-infrastructure-architectures) | EC2 + RDS, serverless API, event-driven processing, Auto Scaling, ECS Fargate, and static delivery | Choosing compute patterns, Terraform, network boundaries, security controls, and scalable design |
| [AWS Terraform Infrastructure](https://github.com/titoiunit/aws-terraform-infrastructure) | Terraform, remote state, Docker, GitHub Actions OIDC, and Amazon ECR delivery | Reusable IaC, environment separation, short-lived cloud credentials, and repeatable delivery |

## Supporting work in active development

| Project | Current scope | How I present it |
|---|---|---|
| [Azure Hands-on Projects](https://github.com/titoiunit/azure-hands-on-projects) | Cost-aware cross-cloud lab workstreams: storage, VMs, Functions, events, containers, monitoring, and Terraform | A learning path; an item becomes featured only after code, evidence, operations notes, and cleanup instructions exist |
| [Python Backend Deployment Scaffold](https://github.com/titoiunit/python-production-backend-template) | A small workload scaffold for future container, CI, and cloud deployment practice | Not presented as a production API until the implementation and CI evidence are in the repository |

## Engineering approach

```text
Understand the workload
→ assess security, availability, and cost constraints
→ design the smallest appropriate architecture
→ implement with Terraform and version control
→ validate deployment and failure paths
→ add observability and document operations
→ clean up temporary resources
```

A working deployment alone is not the finish line; the project must also be explainable, maintainable, and cost-conscious.

## Evidence standard

Each completed project is documented against the same standard:

1. **Problem and constraints** — what the workload needed and what was deliberately out of scope.
2. **Architecture and decisions** — services used, alternatives considered, and key trade-offs.
3. **Implementation** — Terraform, application, or automation components.
4. **Security and operations** — IAM, network boundaries, logging, alarms, and failure handling.
5. **Validation** — how the deployment and important paths were tested.
6. **Cost and cleanup** — guardrails, resources to destroy, and proof of safe teardown.
7. **Interview summary** — a concise explanation of business value and engineering choices.

The reusable [Portfolio Lab Standard](lab-standards/README.md) is the definition of “done.”

## Current depth-building roadmap

The next labs are prioritised in the [cost-aware roadmap](roadmap/README.md): private AWS service access, event-driven hardening, CloudWatch operations, secrets rotation, safe ECS releases, recovery testing, and then time-boxed Kubernetes/edge-security validation.

## Repository map

- `architecture-maps/` — cross-cloud and service-pattern comparisons
- `case-studies/` — deeper explanations of implemented work
- `interview-notes/` — concise, evidence-based interview narratives
- `lab-standards/` — the reusable definition of done
- `roadmap/` — planned work, explicitly separated from shipped portfolio evidence

## Status

Active portfolio. I build the implementation first, then publish the architecture, validation evidence, and operational notes that support it.