# Designing Application Deployments in Various Environments

This directory contains the Docker data files used in the demos.
The `Dockerfile` describes the image itself, and `docker-compose.yml`
is a simple automation tool for building multiple docker containers.
The CRM app is containerized as a single entity.
A more professional (read: advanced) strategy would be to break up
the model, view, and controller components into separate containers.

## Setup files
Basic Bash scripts to expedite the installation of Docker as
such tasks are administrative in nature.
These files are contained in the `setup/` directory.
  * `centos7_docker_install.sh`: Installs Docker on CentOS 7. Run as `sudo`.
  * `docker_compose_install.sh`: Installs `docker-compose`. Run as `sudo`.

## Bash aliases for CentOS 7 installs

Bash aliases may simplify using `docker` from the shell.

```
alias dc='sudo docker container'
alias di='sudo docker image'
alias db='sudo docker build'
alias comp='sudo docker-compose'
```
