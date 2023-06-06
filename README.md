# Curso de Docker para la Dirección de Información Geoespacial

Este repositorio tiene el objetivo resguardar distintos ejemplos de herramientas útiles para el desarrollo orientado a la DIG.
Se compone de distintos directorios con recetas de imágenes de Docker.

## Jupyter Minimal Notebook (jupyter_minimal_notebook)

Jupyter Docker Stacks are a set of ready-to-run [Docker images](https://hub.docker.com/u/jupyter) containing Jupyter applications and interactive computing tools.
You can use a stack image to do any of the following (and more):

- Start a personal Jupyter Server with the JupyterLab frontend (default)
- Run JupyterLab for a team using JupyterHub
- Start a personal Jupyter Notebook server in a local Docker container
- Write your own project Dockerfile

We are going to use Jupyter Minimal Notebook from the all set of this stack.

[jupyter/minimal-notebook](https://hub.docker.com/r/jupyter/minimal-notebook) adds command-line tools useful when working in Jupyter applications.

It contains:

- Everything in jupyter/base-notebook
- Common useful utilities like git, nano (actually nano-tiny), tzdata, unzip and vi (actually vim-tiny),
- TeX Live for notebook document conversion

En el sitio web [towardsdatascience](https://towardsdatascience.com/how-to-run-jupyter-notebook-on-docker-7c9748ed209f) pueden ver un tutorial completo de cómo desplegar jupyter/minimal-notebook

## Postgres with Postgis (postgres_postgis)

The [postgis/postgis](https://hub.docker.com/r/postgis/postgis) image provides tags for running Postgres with PostGIS extensions installed. This image is based on the official postgres image and provides debian and alpine variants for PostGIS 3.3.x for each supported version of Postgres (11, 12, 13, 14 and 15). Additionally, an image version is provided which is built from the latest two versions of Postgres (14, 15) with versions of PostGIS and its dependencies built from their respective master branches.
