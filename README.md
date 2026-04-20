# Argo Workflows (argo-workflows)
Argo Workflows is an open-source, container-native workflow engine for orchestrating parallel jobs on Kubernetes. It is a CNCF graduated project that allows you to define workflows where each step is a container, model multi-step workflows as sequences of tasks or DAGs, and run compute-intensive jobs for machine learning, data processing, and CI/CD pipelines natively on Kubernetes. Governed by the Linux Foundation and the CNCF.

**URL:** [https://argoproj.github.io/workflows/](https://argoproj.github.io/workflows/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - CNCF, Containers, Data Processing, Kubernetes, Machine Learning, Open Source, Workflow Engine

## Timestamps

- **Created:** 2026-03-27
- **Modified:** 2026-04-19

## APIs

### Argo Workflows API
The Argo Workflows REST API provides programmatic access to workflow lifecycle management, workflow templates, cron scheduling, archived workflow history, events, and cluster workflow templates. Authentication uses JWT bearer tokens from service account secrets.

**Human URL:** [https://argo-workflows.readthedocs.io/en/latest/swagger/](https://argo-workflows.readthedocs.io/en/latest/swagger/)

#### Tags:

 - Kubernetes, REST API, Workflow Engine

#### Properties

- [Documentation](https://argo-workflows.readthedocs.io/en/latest/)
- [OpenAPI](openapi/argo-workflows-openapi.json)
- [GettingStarted](https://argo-workflows.readthedocs.io/en/latest/quick-start/)
- [APIReference](https://argo-workflows.readthedocs.io/en/latest/swagger/)
- [Authentication](https://argo-workflows.readthedocs.io/en/latest/access-token/)

## Common Properties

- [Website](https://argoproj.github.io/workflows/)
- [Documentation](https://argo-workflows.readthedocs.io/en/latest/)
- [GettingStarted](https://argo-workflows.readthedocs.io/en/latest/quick-start/)
- [GitHubOrganization](https://github.com/argoproj)
- [GitHubRepository](https://github.com/argoproj/argo-workflows)
- [ReleaseNotes](https://github.com/argoproj/argo-workflows/releases)
- [ChangeLog](https://argo-workflows.readthedocs.io/en/latest/new-features/)
- [CLI](https://argo-workflows.readthedocs.io/en/latest/cli/)
- [SDK](https://hera.readthedocs.io/en/stable/)
- [Support](https://github.com/argoproj/argo-workflows/issues)

## Features

| Name | Description |
|------|-------------|
| Container-Native Workflows | Every workflow step runs as a Kubernetes container, providing complete isolation and reproducibility. |
| DAG and Step-Based Orchestration | Define multi-step workflows as sequential steps or directed acyclic graphs (DAGs) with dependencies. |
| Parallel Execution | Run multiple workflow steps in parallel to maximize compute utilization and reduce execution time. |
| Workflow Templates | Store and reuse workflow definitions as templates across the cluster. |
| Cron Workflows | Schedule workflows to run on cron schedules directly on Kubernetes. |
| Artifact Support | Pass artifacts between workflow steps via S3, GCS, Azure Blob, Artifactory, and more. |
| Workflow Archive | Persist workflow history to a database for long-term retention and querying. |
| Web UI | Monitor and manage workflows through a rich graphical interface. |
| Multi-Tenancy | Namespace-based isolation with RBAC for multi-team environments. |
| Event-Driven Triggers | Trigger workflows from Kubernetes events, webhooks, and custom event sources. |
| Python SDK (Hera) | Define workflows in Python using the Hera SDK, the official Python SDK. |
| Plugin Architecture | Extend with custom executor plugins and artifact driver plugins. |

## Use Cases

| Name | Description |
|------|-------------|
| Machine Learning Pipelines | Orchestrate data preparation, model training, evaluation, and deployment as containerized steps. |
| Data Processing and ETL | Run parallel data transformation and ETL jobs at scale on Kubernetes. |
| CI/CD on Kubernetes | Run CI/CD pipelines natively on Kubernetes without external CI tools. |
| Batch Processing | Process large datasets in parallel with automatic resource management. |
| Infrastructure Automation | Automate infrastructure provisioning, testing, and validation workflows. |
| Scientific Computing | Orchestrate complex scientific computation and simulation jobs with dependencies. |

## Integrations

| Name | Description |
|------|-------------|
| Python Hera SDK | Official Python SDK for defining and submitting workflows programmatically. |
| Argo CD | Use Argo CD to deploy and manage Argo Workflows resources via GitOps. |
| Prometheus | Expose workflow metrics for Prometheus monitoring and alerting. |
| Grafana | Visualize workflow performance metrics in Grafana dashboards. |
| HashiCorp Vault | Inject secrets into workflow containers securely via Vault integration. |
| Amazon S3 | Use S3 as artifact storage for passing data between workflow steps. |
| Google GCS | Use Google Cloud Storage as artifact backend. |
| Azure Blob Storage | Use Azure Blob Storage for artifact persistence. |
| Kubeflow | Run Kubeflow ML pipelines using Argo Workflows as the underlying engine. |
| Apache Spark | Orchestrate Apache Spark jobs as Argo Workflow steps. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Argo Workflows OpenAPI](openapi/argo-workflows-openapi.json)

### JSON Schema

421 schema files in [json-schema/](json-schema/)

### JSON Structure

421 structure files in [json-structure/](json-structure/)

### JSON-LD

7 context files in [json-ld/](json-ld/)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [Argo Workflows API](capabilities/shared/argo-workflows-api.yaml) — 5 operations for workflow, template, cron, and archive management

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Workflow Orchestration](capabilities/workflow-orchestration.yaml) | Argo Workflows | 5 | Data Engineer, Platform Engineer |

## Vocabulary

- [Argo Workflows Vocabulary](vocabulary/argo-workflows-vocabulary.yaml) — Unified taxonomy mapping 7 resources, 11 actions, 1 workflow, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Argo Workflows Spectral Rules](rules/argo-workflows-spectral-rules.yml) — 13 rules across 5 categories enforcing Argo Workflows API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
