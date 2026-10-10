FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:a8256f4a2c8a38bdcf26164d372eedfcd02cb15e048b124f0d5b075a0d1e405d

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
