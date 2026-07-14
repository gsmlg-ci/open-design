# open-design

[![Build](https://github.com/gsmlg-ci/open-design/actions/workflows/build.yml/badge.svg)](https://github.com/gsmlg-ci/open-design/actions/workflows/build.yml)

Docker image for [nexu-io/open-design](https://github.com/nexu-io/open-design), built from the upstream `deploy/Dockerfile`.

Docker image published to:
- `docker.io/gsmlg/open-design`
- `ghcr.io/gsmlg-dev/open-design`

## Usage

```bash
# From Docker Hub
docker pull gsmlg/open-design:latest

# From GitHub Container Registry
docker pull ghcr.io/gsmlg-dev/open-design:latest
```

Open Design listens on port `7456` by default.

```bash
docker run --rm -p 127.0.0.1:7456:7456 gsmlg/open-design:latest
```

## Build

```bash
docker build -t gsmlg/open-design -f deploy/Dockerfile https://github.com/nexu-io/open-design.git#main
```
