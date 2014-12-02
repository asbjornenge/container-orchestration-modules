# Container Orchestration Modules

> Applying the [UNIX philosophy](http://en.wikipedia.org/wiki/Unix_philosophy) to container orchestration.

This repository is an attempt at identifying & describing the different parts of doing container orchestration, and supplying information about single purpose tools, libraries and techniques to solve each part.

**DISCLARIMER** You will find an abundance of [nodejs](http://nodejs.org/) related tools.  

**PS!** There are many missing tools, libraries, descriptions and even whole parts in this document. Please help by opening issues and sending pull requests :santa: :package: :+1:

## Configuration

Describe your containers and the relationships between them.

* [common-container-configuration-format](https://github.com/asbjornenge/common-container-configuration-format) - Common Container Configuration Format

### Wanted Modules

* Configuration X -> cccf parsers
* Docker cccf module (adding docker specific links, volumes_from, etc.)
* Cluster cccf module (adding scale etc.)
* Resources cccf module (adding resource requirements etc.)
* Host cccf module(s) (adding a container host - in a multi-host setup this would be useful)

## Distribution

Distribute your container images for hosts to find them.

* [torrent-docker](https://github.com/mafintosh/torrent-docker) - MAD SCIENCE realtime boot of remote docker images using bittorrent
* [docker-registry-server](https://github.com/mafintosh/docker-registry-server) - docker registry server in node.js

## Service Discovery

How your containers discover each other and exchange information about themselves.

* [rainbow-dock](https://github.com/asbjornenge/rainbow-dock) - DNS based service discovery for docker

## Scheduling

A process for determining what containers are run and where.

### Notes

Scheduling is a quite complex matter and can have many layers. We would be smart to build a composable toolchain here.

## Management

How containers are managed over time.

### Notes

WANTED: A React.js style state management tool. I have state X but now I want state Y, make me a list operations to achieve this.

## Monitoring

How containers are monitored and watched.
