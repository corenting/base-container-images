FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:52b81a56c3fe8fce762bd02699eba3c36a5efee695f685d6d90db3272c06854c

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
