# 9. Configuration Management Policy

Postie standardizes and automates configuration management through the use of AWS Data Pipeline and Elastic Beanstalk deployments as well as documentation of all changes to production systems and networks.

## 9.1 Applicable Standards

### 9.1.1 Applicable Standards from the HITRUST Common Security Framework

* 06 - Configuration Management

### 9.1.2 Applicable Standards from the HIPAA Security Rule

* 164.310(a)(2)(iii) Access Control & Validation Procedures

## 9.2 Configuration Management Policies

1. Elastic Beanstalk and Ops Works is used to standardize and automate configuration management.
2. No systems are deployed into Postie environments without approval of the Postie CTO.
3. All changes to production systems, network devices, and firewalls are approved by the Postie CTO before they are implemented to assure they comply with business and security requirements.
4. All changes to production systems are tested before they are implemented in production.
5. Implementation of approved changes are only performed by authorized personnel.
6. All committed code is reviewed to assure software code quality and proactively detect potential security issues in development.
7. Postie deploys environments locally using Vagrant to assure functionality before moving to staging or production.

## 9.3 Patch Management Procedures

1. Postie uses automated tooling to ensure systems are up-to-date with the latest security patches.
2. On Ubuntu Linux systems, the unattended-upgrades tool is used to apply security patches in phases.