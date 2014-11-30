# Docker Orchestration Modules

> Applying the [UNIX philosophy](http://en.wikipedia.org/wiki/Unix_philosophy) to [docker](https://www.docker.com/) orchestration.

This repository is an attempt at identifying & describing the different parts of doing docker orchestration, and supplying information about single purpose tools, libraries and techniques to solve each part.

**DISCLARIMER** You will find an abundance of [nodejs](http://nodejs.org/) related tools.  

**PS!** There are many missing tools, libraries, descriptions and even whole parts in this document. Please help by opening issues and sending pull requests :santa: :package: :+1:

## Configuration

Describe your containers and the relationships between them.

TODO: What could this look like in terms of modules?

### Missing Modules

* Configuration parser
* Common format?

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

How container are monitored and watched.