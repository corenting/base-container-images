FROM ghcr.io/corenting/base-container-images/python-3.14:latest@sha256:e83fad820aaa55d7b076ea5f7571b0f90f7f84c4dfd41004988f3eb41899ff7b

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
