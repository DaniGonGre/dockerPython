# Docker + Python

---
# Creamos un contenedor sencillo de python

`$ docker run -it --rm -v "$PWD":/usr/src/myapp -w /usr/src/myapp python:3 python script.py`

`docker` el comando base, es el daemon

`run` crear el contenedor

`-it` dos opciones que me valen para interectuar con la terminal del contenedor

`--rm` borra el contenedor cuando finaliza la acción

`-v` define el mapeo del volumen a continuación

- `$PWD` el directorio donde estamos
- `/usr/src/myapp` el directorio dentor del contenedor

`-w` el directorio de trabajo (_workdir_)

`python:3` es la imagen de la que se creará el contenedor

`python script.py` es el comando para ejecutar dentro del contenedor

