FROM ghcr.io/corenting/base-container-images/python-3.14:latest@sha256:38d60d2c817be5b87a8ca4a636a7aba04904d68dc2f5384bb7ba5d94a64a1438

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
