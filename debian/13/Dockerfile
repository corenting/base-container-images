# Python system base
FROM debian:13@sha256:34cd9e9fd437c0a095ec39cb2e73422c9f30821b0d0848ed74fd0d43bae4d958 AS base

# renovate: depName=dumb-init
ARG DUMB_INIT_VERSION=1.2.5-3

# Install dependencies and dumb-init
RUN apt-get update && apt-get install -y --no-install-recommends dumb-init=${DUMB_INIT_VERSION} && rm -rf /var/lib/apt/lists/*

# Create a nonroot user and an /app directory for installation
RUN useradd --system --no-create-home nonroot && mkdir /app && chown -R nonroot:nonroot /app

USER nonroot

WORKDIR /app

ENTRYPOINT ["dumb-init", "--"]
