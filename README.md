# Creación de un sitio web estático con MkDocs y GitHub Pages

Para crear un sitio con MKDocs lo vamos a hacer a través de contenedores de docker, por lo que necesitaremos docker y docker-compose instalado.

Una vez instalados ejecutamos el comando `docker run --rm -it -p 8000:8000 -v "$PWD":/docs squidfunk/mkdocs-material new proyecto`, el cual nos creará una nueva carpeta llamada proyecto en donde se alojará la página.

Una vez descargado modificamos el archivo mkdocs.ymk con los siguientes parámetros:

![mkdocs](https://raw.githubusercontent.com/arr588/iaw-mkdocs/main/img/1.png)

Con todo esto hecho iniciamos la página con `docker run --rm -it -p 8000:8000 -v "$PWD":/docs squidfunk/mkdocs-material`.