# Pterodactyl-Java-Eggs

## Overview

This project contains Docker images for use with Pterodactyl. It includes various versions of Java, ensuring that the images work on different platforms such as `linux/amd64` and `linux/arm64`.

## Directory Structure

- `.github/workflows/Java.yml`: GitHub Actions workflow for building and publishing the Java Docker images.
- `java/entrypoint.sh`: Entrypoint script executed when the Java container starts.
- `java/21/Dockerfile`: Dockerfile for Java 21.

## Docker Images

The Docker images are automatically built and pushed to the GitHub Container Registry (`ghcr.io`). The tags of the images follow the schema `java_<version>`.

## Usage

### Running a Docker Image

To run a Docker image, use the following command:

```sh
docker run -it ghcr.io/coho04/pterodactyl-docker-images:java_<version>
```