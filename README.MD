# Patatman HASS Config 🍟

Basic Home Assistant config, with regular updates

<img align="right" src="./.assets/logo.png?raw=true" height="170">

- over 20 different components
- Updated love-lace
- Minimal custom components, so it just works! 
- Simple automations
- Tutorials (coming soon!)

[![Build Status](https://travis-ci.org/patatman/patatman-homeassistant-config.svg?branch=master)](https://travis-ci.org/patatman/patatman-homeassistant-config)
[![GitHub Last Commit](https://img.shields.io/github/last-commit/patatman/patatman-homeassistant-config.svg)](https://img.shields.io/github/last-commit/patatman/patatman-homeassistant-config.svg)
[![HA Version](https://img.shields.io/badge/Home%20Assistant-0.84.6-blue.svg)](https://img.shields.io/badge/Home%20Assistant-0.84.6-blue.svg)

## Installation
First clone the repo: 
```
$ git clone https://github.com/patatman/patatman-homeassistant-config.git
```
Next, edit the docker-compose file to match our enviroment. More about docker-compose here: [Docker](https://www.home-assistant.io/docs/installation/docker/)
Then move the `docker-compose.yml` file one folder up.
```
$ cp docker-compose.yml ../docker-compose.yml
```
This is needed since we're mounting the whole directory as our config.

If you'd only like to use a certain compenent, just copy the configuration to your own configuration, and create a Frankensteie config (made up of bits and pieces of everyone's configuration)

## Usage

<img align="right" src="./.assets/hass-docker-compose.gif?raw=true">


## Hardware
To see a full list of Hardware, please see [Components](./components.md)
### Server
 ### Hardware
 - Intel core i3-6100
 - 16GB Ram
 - 256GB SSD
 - 4 TB disk
## Software
 - Hyperviser: Proxmox
 - VM's: 2
   - Docker
   - other (influx, grafana etc)



