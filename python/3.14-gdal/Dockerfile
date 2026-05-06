FROM ghcr.io/corenting/base-container-images/python-3.14:latest@sha256:2b35ded15f213b56f1830270bc4a8c3ae3040e17009f7797cfeb1c7465ecabcc

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
