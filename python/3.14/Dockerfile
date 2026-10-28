# Python system base
FROM python:3.15.2-trixie@sha256:b9dc13dd9e9c69543a3a8ae44ecae5f6a17ddd45f52ac335315de0ff1d9a67ae AS base

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
