FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:af45db46a941b9da976b3b695bccd88cfba6db5e3cebcf6b0fab4104014d5a20

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
