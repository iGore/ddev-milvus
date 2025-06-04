[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/iGore/ddev-milvus/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/iGore/ddev-milvus/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/iGore/ddev-milvus)](https://github.com/iGore/ddev-milvus/commits)
[![release](https://img.shields.io/github/v/release/iGore/ddev-milvus)](https://github.com/iGore/ddev-milvus/releases/latest)

# DDEV Milvus

## Overview

This add-on integrates Milvus into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get iGore/ddev-milvus
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Milvus |
| `ddev logs -s milvus` | Check Milvus logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.milvus --milvus-docker-image="busybox:stable"
ddev add-on get iGore/ddev-milvus
ddev restart
```

Make sure to commit the `.ddev/.env.milvus` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `MILVUS_DOCKER_IMAGE` | `--milvus-docker-image` | `busybox:stable` |

## Credits

**Contributed and maintained by [@iGore](https://github.com/iGore)**
