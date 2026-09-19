FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:1998f90a52c9459fe2309011223386080b9133ecf096b134efb2d79aa72d0201

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
