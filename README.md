# Container Orchestration Modules

> Applying the [UNIX philosophy](http://en.wikipedia.org/wiki/Unix_philosophy) to container orchestration.

This repository is an attempt at identifying & describing the different parts of doing container orchestration, and supplying information about single purpose tools, libraries and techniques to solve each part.

**DISCLARIMER** You will find an abundance of [nodejs](http://nodejs.org/) related tools.  

**PS!** There are many missing tools, libraries, descriptions and even whole parts in this document. Please help by opening issues and sending pull requests :santa: :package: :+1:

## Configuration

Describe your containers and the relationships between them.

* [cccf](https://github.com/asbjornenge/cccf) - Common Container Configuration Format
* [cccf-docker-instructions](https://github.com/asbjornenge/cccf-docker-instructions) - Generate docker cli instructions from a cccf config
* [cccf-scale](https://github.com/asbjornenge/cccf-scale) - Scale up/down a cccf config

## Distribution

Distribute your container images for hosts to find them.

* [torrent-docker](https://github.com/mafintosh/torrent-docker) - MAD SCIENCE realtime boot of remote docker images using bittorrent
* [docker-registry-server](https://github.com/mafintosh/docker-registry-server) - docker registry server in node.js

## Service Discovery

How your containers discover each other and exchange information about themselves.

* [rainbow-dock](https://github.com/asbjornenge/rainbow-dock) - DNS based service discovery for docker

## Scheduling

A process for determining what containers are run and where.

* [cccf-host-basic](https://github.com/asbjornenge/cccf-host-basic) - Extremely basic example of spreading containers across multiple hosts. Serves mostly as a basic example of an cccf-host-x modules.
* We need more cccf-host-x modules!

## Management

How containers are managed over time.

* [cccf-diff](https://github.com/asbjornenge/cccf-diff) - Diff two cccf configs

## Monitoring

How containers are monitored and watched. Alerts?

## Wanted Modules

**cccf-docker**  
Extend cccf with docker specific fields (links, volumes_from, etc.).

**docker-cccf**    
docker ps / inspect -> cccf-docker format
