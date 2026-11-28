FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:2fcaf60ce5543d2a8bbd04bcb9a85b965d5286d53ec5660091f01b63e2f08ca7

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
