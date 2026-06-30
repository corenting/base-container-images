FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:3ab89b76afbb27eff72f9121aba3d7f5d6aee0925a1f047e9d9696a09829e3ec

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
