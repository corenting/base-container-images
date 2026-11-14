FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:0165285303b867b3e9aa9d93321bda2ee2cb51f3433a629b8631d2fb6dfcc8bc

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
