# Clever Cloud workshop

A hands-on path to deploy applications on Clever Cloud, from a first "hello world" to managed authentication and infrastructure as code. Each step is a small, self-contained application in its own repository, included here as a Git submodule.

```bash
git clone --recurse-submodules https://github.com/vballu/clever-cloud-workshop.git
```

## Steps

| Step | Folder | What you learn |
|---|---|---|
| 0 | [`0-hello-world`](https://github.com/CleverCloud/demo-python-hello-world-uv) | Deploy a Python (Flask, uv) application with `git push` and Clever Tools |
| 1 | [`1-minichat-keycloak`](https://github.com/CleverCloud/demo-python-uv-minichat-keycloak) | Add a managed PostgreSQL database, then protect the chat with a Keycloak add-on |
| 2 | [`2-secure-chat`](https://github.com/vballu/clever-cloud-demo-secure-chat) | A hardened chat behind Keycloak, deployed with Clever Tools or with Terraform/OpenTofu (`terraform/`) |
| 3 | [`3-bonus-ocr`](https://github.com/CleverCloud/demo-python-uv-mini-ocr) | A small OCR micro-service (Tesseract) with Basic Auth |

Going further: [data lake tutorials on Clever Cloud](https://github.com/CleverCloud/data-lake-tutorials) (DuckDB, Trino, Spark, Iceberg, DuckLake and Delta Lake on Cellar).

## Before you start

- A Clever Cloud account and [Clever Tools](https://www.clever.cloud/developers/doc/cli/) (`clever login`).
- [uv](https://docs.astral.sh/uv/) for the Python steps, and Terraform or OpenTofu for the infrastructure-as-code option of step 2.

## Updating the steps

Each folder points to a fixed commit of its repository. To move every step to its latest version:

```bash
git submodule update --remote
```

## Author

Victor Ballu, pre-sales engineer and data scientist at Clever Cloud.
