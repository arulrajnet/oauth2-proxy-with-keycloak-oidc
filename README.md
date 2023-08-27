# OAuth2 Proxy with Keycloak as Provider

This repo for securing your web application with OAuth2 Proxy and Keycloak as IDP.

The architecture is look like this:

![Architecture](./assets/architecture.drawio.svg)

## Pre-requisites

- Docker
- Docker Compose

## How to run

1. Clone this repo
2. Run `docker-compose up -d`
3. Map the `SERVER_FQDN` domain to `/etc/hosts` or `/c/Windows/System32/drivers/etc/hosts` file
3. Open your browser and go to `http://<SERVER_FQDN>`
