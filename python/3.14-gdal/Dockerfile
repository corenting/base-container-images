FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:54e5c66d099dc2d18df1eb14c494ef679555c4795e24460efb1d3d779dabbd70

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
