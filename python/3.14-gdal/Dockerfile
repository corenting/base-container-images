FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:bd4c80fda72a22ab7a729752efd794a6d7d5cbaf293534a4cde50771d1d382d4

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
