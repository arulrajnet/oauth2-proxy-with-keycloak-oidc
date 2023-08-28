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


To logout

http://demo.arulraj.net/oauth2/sign_out?rd=http%3A%2F%2Fdemo.arulraj.net%2Fauth%2Frealms%2Fdemo%2Fprotocol%2Fopenid-connect%2Flogout%3Fredirect_uri%3Dhttp%3A%2F%2Fdemo.arulraj.net%2F


## TODO

- [ ] Set password for create user via keycloak cli
- [ ] Fix logout redirect URI
- [ ] First name and last name as header
- [ ] Expose first name and last name in userinfo endpoint
