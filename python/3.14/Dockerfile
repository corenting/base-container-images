# Python system base
FROM python:3.14.8-trixie@sha256:a11116e648ddd8a05e1120014c8e6ac259f718040b67e2dcd6a7c0b7bab3ff2c AS base

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
