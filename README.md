# libretro-netplay-registry

Stores a netplay registry for libretro.

## Usage

- Retrieve all entries in registry.lpl by visiting index.php
- Add an entry by requesting index.php?username=<user>&ip=<ip>&corename=<corename>&coreversion=<coreversion>&gamename=<gamename>&gamecrc=<gamecrc>

## Install

1. Check out the git repository
1. Make sure SQLite3 is available to PHP
1. Make sure .registry.sqlite is writable by PHP
1. Visit index.php and see that the registry is empty
1. Visit index.php?username=<user>&ip=<ip>&corename=<corename>&coreversion=<coreversion>&gamename=<gamename>&gamecrc=<gamecrc> to add an entry
1. Visit index.php and see your new entry added

## Development

Use [Docker Compose](https://docs.docker.com/compose/) to set up a development environment. Instructions are in [docker-compose.yml](docker-compose.yml).

## TODO

- Add some validation and security behind adding entries

## Hosting

The server, hosted at http://lobby.libretro.com is running the following software:

- PHP 5.5.9
- SQLite3
- Apache
