# Python system base
FROM python:3.14.3-trixie@sha256:dae380cbff69335514b37adbf4d30d143d230f155caf752051c99a3d8133da4b AS base

# renovate: depName=dumb-init
ARG DUMB_INIT_VERSION=1.2.5-3

# Install dependencies and dumb-init
RUN apt-get update && apt-get install -y --no-install-recommends dumb-init=${DUMB_INIT_VERSION} && rm -rf /var/lib/apt/lists/*

# Environment
ENV PYTHONUNBUFFERED=1 \
    PYTHONDONTWRITEBYTECODE=1

# Create a nonroot user and an /app directory for installation
RUN useradd --system --no-create-home nonroot && mkdir /app && chown -R nonroot:nonroot /app

USER nonroot

WORKDIR /app

ENTRYPOINT ["dumb-init", "--"]
