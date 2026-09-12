FROM ghcr.io/corenting/base-container-images/python:3.14@sha256:dfde4920e92c879035f41b4afb9dfcbf2a5938c067115f1bdea74b1f7272e9b3

USER root

# Install GDAL
RUN apt-get update && apt-get install -y --no-install-recommends gdal-bin libgdal-dev && rm -rf /var/lib/apt/lists/*

USER nonroot
