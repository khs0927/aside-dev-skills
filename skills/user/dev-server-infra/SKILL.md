---
name: "dev-server-infra"
description: "Use for servers, Linux, cloud AWS Azure GCP, networking, Docker, Kubernetes, Terraform, CI-CD, deployment, observability, or security hardening."
---
# Dev Server Infra

Operate infrastructure with reproducible configs and safe defaults.

## Workflow

1. Identify target: OS, cloud, runtime, network, and data store.
2. Prefer infrastructure-as-code: Terraform/OpenTofu, containers, systemd, or CI YAML.
3. Apply least privilege: non-root, read-only filesystem where possible, scoped secrets.
4. Add observability: logs, metrics, health checks, and alerts for every service.
5. Verify: dry-run or plan first, then deploy, smoke-test, and roll back on failure.
6. Document endpoint, ports, env vars, and runbook steps.

## Decision rules

- Never paste secrets into code, logs, or chat; use vault or env injection.
- Prefer managed services for DB, DNS, CDN unless self-hosting is required.
- For Kubernetes: set requests/limits, probes, resource quotas, and securityContext.
- For SSH/Linux: key auth, bastion where needed, minimal sudo, audit users.
- For releases: use staged rollout and CI gates before production.

## Examples

- "Deploy Node API": Dockerfile, health endpoint, env config, reverse proxy, TLS, logs.
- "Debug high CPU": check metrics, top processes, slow endpoints, scale or tune.
- "Add Terraform for S3": versioned module, plan output, least-privilege IAM.

## References reviewed

- BagelHole/DevOps-Security-Agent-Skills server, cloud, IaC, and hardening patterns.
- HashiCorp Terraform and OpenTofu migration skills.
- AWS DevOps Agent investigation workflows and reusable skill structure.
- Cloudflare, Netlify, and Vercel deployment skill patterns.




























