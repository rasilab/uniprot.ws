# UniProt.ws Docker Container

This repository contains the Dockerfile for the UniProt.ws R package container.

## Container Details

- **Base Image**: `ghcr.io/rasilab/r_python:1.3.0`
- **Package Version**: UniProt.ws 2.38.0 (Bioconductor)
- **Registry**: `ghcr.io/rasilab/uniprot.ws`

## Usage

```bash
docker pull ghcr.io/rasilab/uniprot.ws:2.38.0
```

## Running the Container

```bash
docker run -it --rm ghcr.io/rasilab/uniprot.ws:2.38.0 bash
source activate R
R
```

## Features

- UniProt.ws R package for accessing UniProt web services
- Configured with Fred Hutch conda proxy
- Installed from bioconda channel

## Building

```bash
docker build -t ghcr.io/rasilab/uniprot.ws:2.38.0 .
```