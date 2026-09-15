FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:9edf962f686c9a369eeda1066fb6035082081a9498c9e3b7b0de1cfb9d41052c

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
