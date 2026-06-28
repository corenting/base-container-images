FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:edb2ef47134cd740ad6ec3df537844cde9a81484e9324a40150a63436836bc77

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
