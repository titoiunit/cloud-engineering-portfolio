# Portfolio Lab Standard

A lab is featured in this portfolio only when it tells the full engineering story, not just when Terraform applies successfully.

## Definition of done

- [ ] Problem and constraints are stated in plain language
- [ ] Architecture diagram shows the request, compute, data and operations flow
- [ ] Terraform or other implementation code is committed and readable
- [ ] Security boundaries and IAM decisions are documented
- [ ] Validation steps prove the important path and one failure or recovery path
- [ ] Logging, metrics and alarms are considered where relevant
- [ ] Cost guardrails and cleanup steps are explicit
- [ ] Trade-offs and a next production-hardening step are included
- [ ] A 30-second interview explanation is written

## README layout

```text
# Project name
## Problem and goal
## Architecture
## Key decisions and trade-offs
## Implementation
## Security and operations
## Validation
## Cost and cleanup
## What I learned
## Next production-hardening step
## Interview version
```

## Evidence, not claims

A completed project should link to the relevant Terraform, application code, workflow, test output or deployment evidence. Planned work belongs in the roadmap, not in the completed-project section.

## Cost discipline

Every cloud lab starts with a cost plan:

1. choose the smallest viable architecture
2. avoid persistent managed services unless the learning goal requires them
3. set a timebox for paid resources
4. tag resources with the project name and owner
5. destroy temporary resources and record the cleanup

This keeps the portfolio practical while still demonstrating production-aware decision making.
