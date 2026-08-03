# Amazon Backup

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
