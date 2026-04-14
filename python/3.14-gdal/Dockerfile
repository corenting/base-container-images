FROM ghcr.io/corenting/base-container-images/python-3.14:latest@sha256:1bc57b48801b532340c2ccb8880f5104aced0b4ac373814def9cc1a723a08c4a

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
