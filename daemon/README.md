# Pterodactyl Daemon

The server control and management daemon built specifically for Pterodactyl Panel.

[![Docker Build Status](https://img.shields.io/docker/build/sfoxdev/pterodactyl-daemon.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/automated/sfoxdev/pterodactyl-daemon.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/pulls/sfoxdev/pterodactyl-daemon.svg?style=flat-square)]()
[![Docker Build Status](https://img.shields.io/docker/stars/sfoxdev/pterodactyl-daemon.svg?style=flat-square)]()

## Usage

The Pterodactyl Daemon needs to have access to the docker host filesystem and the daemon to work correctly. Refer to the main repository link for all information regarding running the pterodactyl panel within docker.

## Required Mounts

`/srv/daemon/config/` - Main configuration directory for the daemon

`/srv/daemon/packs/` - For server packs

`/srv/daemon/scripts/` - For startup scripts

`/srv/daemon-data/` - Server Data

`/tmp/pterodactyl/` - Temp directory

`/var/run/docker.sock` - Requires the docker daemon docket to operate

`/etc/letsencrypt/live/daemon.example.com` - SSL certificates

All mounts are recommended to be mirrored exactly.
