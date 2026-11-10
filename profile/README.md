# Prixy

**Short-lived, fenced, budgeted AWS access for coding agents.**

Prixy lets you point a coding agent at your AWS account without handing it
your real keys or risking a surprise bill.

- **An hour-long session per project.** The agent gets temporary credentials
  through a normal AWS profile, so the AWS CLI, Terraform, CDK and the SDKs
  keep working unchanged.
- **The fence is IAM, not a prompt.** What the agent may do is enforced by AWS
  itself. It can read what exists, but can only change what it created.
- **Everything it creates is tagged and recorded.**

## Status

Early. Sign-in, connecting an AWS account and issuing fenced credentials work,
and the fence has been tested against a real AWS account. Budgets, plan pricing
and cleanup are not built yet.

The code is private for now.
