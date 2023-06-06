# Jupyter Minimal Notebook (jupyter_minimal_notebook)

## C'po'mo crear la imagen

`docker image build -t jupyter-notebook-dig .`

## Cómo desplegar

`docker container run -p 18888:8888 -v .\workspace\:/home/jovyan --name jupyter-notebook-dig-01 jupyter-notebook-dig`

## Cómo desplegar en segundo plano (y obtener el token)

```
docker container run -d -p 18888:8888 -v .\workspace\:/home/jovyan --name jupyter-notebook-dig-01 jupyter-notebook-dig

docker container logs jupyter-notebook-dig-01
```

## Cómo utilizar

Ingresando a http://localhost:18888/?token=<token> en un navegador web.
El token se imprime por pantalla al desplegar el contenedor o se consulta en el log del contenedor.

## Cómo eliminar el contenedor

```
docker container stop jupyter-notebook-dig-01

docker container rm jupyter-notebook-dig-01
```
