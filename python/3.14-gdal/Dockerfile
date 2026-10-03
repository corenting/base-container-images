FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:a058b9418b39d7831f8a55ffebf7502a705c15a97ca1d031afeffd402040ace4

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
