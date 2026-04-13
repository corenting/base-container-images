FROM ghcr.io/corenting/base-container-images/python-3.14:latest@sha256:e81276923d9db29bbee561dd2552c9c0ad977a7c135a61f7aa2bb87e3e51905b

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
