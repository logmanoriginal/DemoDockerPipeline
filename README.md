# DemoDockerPipeline
Demonstrates building and running docker containers as part of a build pipeline.

This repository is intended for use on self-hosted Windows agents on Azure Pipelines.

# Pipelines
| Pipeline | Status | Link |
|----------|--------|------|
| [hello-world](hello-world.yml) | ![Build Status](https://img.shields.io/azure-devops/build/neuperger/public/23/main?style=flat-square&logo=azure-pipelines&) | [View](https://dev.azure.com/neuperger/Public/_build?definitionId=23&_a=summary) |
| [sshd](sshd.yml) | ![Build Status](https://img.shields.io/azure-devops/build/neuperger/public/24/main?style=flat-square&logo=azure-pipelines&) | [View](https://dev.azure.com/neuperger/Public/_build?definitionId=24&_a=summary) |

# Pre-requisites
- Self-hosted Windows Agent
  - Configured to run as `NETWORK SERVICE` (recommended).
- Docker Desktop
  - `NETWORK SERVICE` added to `docker-users` group: https://stackoverflow.com/a/76952351

> [!NOTE]
> Docker may require firewall rules to allow traffic on the Docker subnet. Observe any prompts during the execution of the pipeline.
