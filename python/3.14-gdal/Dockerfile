FROM ghcr.io/corenting/base-container-images/python-3.14:latest@sha256:137276016400a39a75439f2066400f1b22121bbc46af23898892621b342af24a

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
