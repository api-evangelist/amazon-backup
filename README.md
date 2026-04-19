# Amazon Backup

AWS Backup is a fully managed backup service that centralizes and automates the backup of data across AWS services, enabling you to configure backup policies, monitor backup activity, and restore resources with a single, unified console and API.

**Human URL:** [https://aws.amazon.com/backup/](https://aws.amazon.com/backup/)

**API Reference:** [https://docs.aws.amazon.com/aws-backup/latest/devguide/API_Reference.html](https://docs.aws.amazon.com/aws-backup/latest/devguide/API_Reference.html)

## APIs

### Amazon Backup API

API for centrally managing and automating backups across AWS services including Amazon EBS, Amazon RDS, Amazon DynamoDB, Amazon EFS, Amazon FSx, Amazon EC2, and AWS Storage Gateway.

**Base URL:** `https://backup.us-east-1.amazonaws.com`

#### Key Operations

| Operation | Description |
|---|---|
| CreateBackupPlan | Create an automated backup plan with schedule and lifecycle |
| CreateBackupVault | Create a secure container for recovery points |
| CreateBackupSelection | Assign resources to a backup plan |
| StartBackupJob | Manually trigger a backup job |
| StartRestoreJob | Restore a resource from a recovery point |
| StartCopyJob | Copy a recovery point cross-region |
| CreateLegalHold | Preserve recovery points from deletion |
| CreateFramework | Create a compliance governance framework |
| CreateRestoreTestingPlan | Automate periodic restore validation tests |

## Features

- **Automated Backup Scheduling** — Cron-based schedules with configurable start and completion windows
- **Lifecycle Management** — Automatically transition to cold storage and delete after retention period
- **Cross-Region Copy** — Replicate backups across AWS regions for disaster recovery
- **Cross-Account Management** — Centrally manage backup policies via AWS Organizations
- **Vault Lock (WORM)** — Write-once-read-many protection for regulatory compliance
- **Legal Holds** — Preserve recovery points during legal proceedings
- **Compliance Frameworks** — Automated governance controls and reporting
- **Automated Restore Testing** — Periodic restore validation with compliance reporting
- **Continuous Backup (PITR)** — Point-in-time recovery for supported services

## Use Cases

- **Enterprise Backup Automation** — Tag-based resource selection with centralized policy management
- **Regulatory Compliance** — Vault Lock, frameworks, and automated compliance reports
- **Disaster Recovery** — Cross-region replication with validated restore procedures
- **Legal Hold Management** — Preserve backup data during legal proceedings

## Supported Resources

Amazon EBS, Amazon EC2, Amazon RDS, Amazon Aurora, Amazon DynamoDB, Amazon EFS, Amazon FSx, Amazon S3, AWS Storage Gateway, Amazon DocumentDB, Amazon Neptune, Amazon Timestream, VMware Cloud on AWS

## Artifacts

| Type | URL |
|---|---|
| OpenAPI Spec | [openapi/amazon-backup-openapi.yml](openapi/amazon-backup-openapi.yml) |
| OpenAPI (APIs.guru) | [https://api.apis.guru/v2/specs/amazonaws.com/backup/2018-11-15/openapi.yaml](https://api.apis.guru/v2/specs/amazonaws.com/backup/2018-11-15/openapi.yaml) |
| JSON Schema | [json-schema/amazon-backup-plan-schema.json](json-schema/amazon-backup-plan-schema.json) |
| JSON Structure | [json-structure/backup-resource-structure.json](json-structure/backup-resource-structure.json) |
| JSON-LD Context | [json-ld/amazon-backup-context.jsonld](json-ld/amazon-backup-context.jsonld) |
| Spectral Ruleset | [spectral/ruleset.yml](spectral/ruleset.yml) |
| Capabilities | [capabilities/capabilities.yml](capabilities/capabilities.yml) |
| Vocabulary | [vocabulary/vocabulary.yml](vocabulary/vocabulary.yml) |
| Examples | [examples/](examples/) |

## Common Properties

| Type | URL |
|---|---|
| Documentation | [https://docs.aws.amazon.com/aws-backup/latest/devguide/](https://docs.aws.amazon.com/aws-backup/latest/devguide/) |
| API Reference | [https://docs.aws.amazon.com/aws-backup/latest/devguide/API_Reference.html](https://docs.aws.amazon.com/aws-backup/latest/devguide/API_Reference.html) |
| CLI Reference | [https://docs.aws.amazon.com/cli/latest/reference/backup/](https://docs.aws.amazon.com/cli/latest/reference/backup/) |
| Pricing | [https://aws.amazon.com/backup/pricing/](https://aws.amazon.com/backup/pricing/) |
| Getting Started | [https://aws.amazon.com/backup/getting-started/](https://aws.amazon.com/backup/getting-started/) |
| Blog | [https://aws.amazon.com/blogs/storage/](https://aws.amazon.com/blogs/storage/) |
| Stack Overflow | [https://stackoverflow.com/questions/tagged/aws-backup](https://stackoverflow.com/questions/tagged/aws-backup) |

## Maintainers

**Kin Lane** — [kin@apievangelist.com](mailto:kin@apievangelist.com)
