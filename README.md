# Docker Swarm Local

## About

The purpose of **Docker Swarm Local** is to speed up development and deployment testing through reduction of overhead. **Docker Swarm Local** is intended to provide all of the services required in order to simulate deploying to Docker Swarm without any of the network depencies (i.e. Bamboo, official Private Registry, and official Swarms).

## Prerequisites

### Install Jupyter
The Demo is written as a Jupyter Notebook. First install Jupyter by following instructions as http://jupyter.org/install. Or, as preferred, install via the Anaconda Distribution: https://www.anaconda.com/download/

### Install Bash Kernal
The Demo is written as a Bash notebook, so we'll need to install the Bash Kernal next as defined in https://github.com/takluyver/bash_kernel

Run the following command to install:
> ```
> pip install bash_kernel
> python -m bash_kernel.install
> ```

## Running Jupyter
From the root of the project directory, run the following command:
> ```
> jupyter notebook
> ```

Jupyter will launch in a Web-browser and you should see jupyter-notebook.ipynb. Select it to open the notebook. Follow allong by running each step in the notebook.

## Services of Docker Swarm Local

* [Registry](https://hub.docker.com/_/registry/)
* [Traefik](https://hub.docker.com/_/traefik/)
* [Docker-Registry-Frontend](https://hub.docker.com/r/konradkleine/docker-registry-frontend/)
* [Portainer](https://hub.docker.com/r/portainer/portainer/)