# Python system base
FROM python:3.14-slim AS base

# Install dependencies and dumb-init
RUN apt-get update && apt-get install -y --no-install-recommends dumb-init && rm -rf /var/lib/apt/lists/*

# Environment
ENV PYTHONUNBUFFERED=1 \
    PYTHONDONTWRITEBYTECODE=1

RUN useradd --system --no-create-home nonroot
USER nonroot

ENTRYPOINT ["dumb-init"]
