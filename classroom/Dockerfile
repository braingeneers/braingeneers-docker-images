# ONBUILD instructions in base-image/Dockerfile are used to
# perform certain actions based on the presence of specific
# files (such as conda-linux-64.lock, start) in this repo.
# Refer to the base-image/Dockerfile for documentation:
# https://github.com/pangeo-data/pangeo-docker-images/blob/master/base-image/Dockerfile

# This is a courtesy of the Pangeo project: A community effort for big data geoscience
ARG PANGEO_BASE_IMAGE_TAG=master
FROM pangeo/base-image:${PANGEO_BASE_IMAGE_TAG}
