FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:da8b2617bde025c6319d19a00f0efec9f795a403fa5f99000187f507b8f16366

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
