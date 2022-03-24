# The Production-Grade Infrastructure Checklist

Based on www.gruntwork.io

## Install
- Install the software binaries and all dependencies
- Tools: Ansible, Bash

## Configure
- Configure the software at runtime
  - Port settings, file paths, users, replication, etc.
- Tools: Ansible, Bash

## Provision
- Provision the infrastructure
  - EC2 instances, load balancers, network topology, security groups, IAM permissions, etc.
- Tools: Terraform, CloudFormation

## Deploy
- Deploy the service on top of the infrastructure. Roll out updates with no downtime (blue-green, rolling, canary, etc.).
- Tools: Scripts, Orchestration tools (ECS, Kubernetes)

## Security
- Encryption in transit (TLS) and on disk, authN, authZ, secrets management, server hardening
- Tools: ACM, EBS Volumes, Vault

## Monitoring
- Availability metrics, business metrics, app metrics, server, events, tracing, alerting
- Tools: CloudWatch, Nagios

## Logs
- Rotate logs on disk. Aggregate logs to central location.
- Tools: Cloudwatch, ELK, Splunk

## Backup/Restore
- DB backups
- Tools: RDS, Elasticache, Lambda

## Networking
- VPCs, subnets, static/dynamic IPs, service discovery, firewalls, DNS, SSH, VPN
- Tools: EIPs, VPCs, Route53, F5

## High Availability
- Withstand outages of individual processes, EC2 instances, services, AZs, and regions.
- Tools: Multi AZ, multi region, replication, ASGs, ELBs, F5

## Scalability
- Scale up/down in response to load. Scale horizontally and/or vertically.
- Tools: ASGs, replication, sharding, caching

## Performance
- Optimize CPU, memory, disk, network, usage. Query tuning. Benchmarking, load testing, profiling.
- Tools: ab, JMeter, LoadRunner

## Cost Optimization
- Pick proper instance types, use spot and reserved instances, use auto scaling, remove unused resources.
- Tools: ASGs, spot instances, reserved instances

## Documentation
- Document code, architecture, and practices. Create playbooks to respond to incidents.
- Tools: README, wiki, Slack

## Tests
- Write automated tests for infrastructure code. Run tests after every commit and nightly.
- Tools: Terratest, GitLab CI/CD

## Maintenance
- Update software. Update tools. Update to latest best practices. Add new features. Fix bugs. Install security patches.
- Tools: Humans, commercial support.
