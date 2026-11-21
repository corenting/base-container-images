FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:eaf455b87c83af8fa07f12c32b64746270ca2587071c35152a16d796be8824d6

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
