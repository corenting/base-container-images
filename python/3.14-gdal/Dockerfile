FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:bfaa4cc1be0771ad47a727bf8ab1e5149dd5c9c2a61ced80fecc320fab990901

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
