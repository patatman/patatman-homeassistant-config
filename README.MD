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

## Docker-compose Usage

<img align="right" src="./.assets/hass-docker-compose.gif?raw=true">

I like to use Docker-compose opposed to a long docker run command. Since it gives me more flexibility in restarting home-assistant. It's also easier to maintain, since it's a single file. 
Some of the basics commands you might already use with docker:
### Start the container in the foreground

```
$ docker-compose run
```   
This runs the container in the foreground, showing all TTY straight into your terminal. Handy for debugging.
To exit, hit `ctrl + c` 
<aside class="notice">
Exiting a container running in the foreground will kill it. Meaning Home Assistant will no longer be active.
</aside>

### Start the container in the background

```
$ docker-compose run -d
```  
With the `-d` parameter you send the TTY to the background. This is the recommended way of running Home Assistant, since you can use your terminal.

### Restart containers
```
$ docker-compose restart
```

### Show running containers
```
$ docker-compose ps
```

### View logs

```
$ docker-compose logs -f
```
This will open the logs, and automatically follow them(showing new entries). 
You can also send it without `-f`, this will not follow the logs. 




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



