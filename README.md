# AWS Static Portfolio Website

A beginner-friendly DevOps project that demonstrates how to build a
responsive static portfolio, host it on Amazon S3, manage infrastructure
with Terraform, and automate validation and deployment using GitHub Actions.

## Project Goals

- Build a responsive website using HTML and CSS.
- Learn Amazon S3 static website hosting.
- Understand IAM permissions and S3 bucket policies.
- Provision AWS infrastructure using Terraform.
- Automate validation and deployment with GitHub Actions.
- Document architecture, security, and cost considerations.

## Architecture

The project has two main flows.

### Website traffic

```mermaid
flowchart TD
    A[Visitor Browser] -->|HTTP request| B[S3 Website Endpoint]
    B --> C[Static HTML CSS and Assets]
    D[S3 Bucket Policy] -. permits public reads .-> B