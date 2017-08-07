# Formación Comandos de Git desde 0

En esta pequeña formación se podrá ver los comandos más básicos e importantes de Git.

## ¿Cómo empezar?

Para empezar crearemos una carpeta básica donde queramos crear nuestro repositorio.
Para seguir usaremos la consola [MINGW64](https://git-scm.com/) que viene por defecto con Git.
```sh
cd {ruta_donde_crear_carpeta}
mkdir {carpeta_a_crear}
```
En esta carpeta no tendremos por ahora Git, es decir, no habrá un repositorio ni nada
que vincule esa carpeta a un control de versiones.

Para solventar este problema, usaremos el siguiente comando:

```sh
git init
```

Con lo que si hacemos ahora un

```
ls -a
```

Veremos que se ha creado una carpeta .git, a partir de ahí ya podremos trabajar con los comandos Git básicos. Destacar que esto es solo un repositorio local, por lo que no estará disponible en los sitios típicos [GitHub](https://github.com/) o [Bitbucket](https://bitbucket.com/).

## Publicar el repositorio.

Para el caso que nos compete, usaremos **GitHub** como sistema de control de versiones.

Una vez inicializado el repositorio abriremos [GitHub Desktop](https://desktop.github.com/) y nos loggearemos con nuestra cuenta de usuario de **GitHub**.

En ***File*** haremos clic en ***Add Local Repository*** y buscaremos el path de la carpeta que hemos creado para esta formación.

Para empezar con un commit inicial, es recomendable crear un archivo llamado README.md con el que se suele explicar la información básica del repositorio, así que crearemos dicho archivo con el contenido siguiente:
```
# Formación Git
```
Y haremos un commit siguiendo los pasos siguientes, estos pasos se suelen repetir mucho en un proyecto por lo que hay que tenerlos por mano.

```
git add README.md
git commit -m "Commit inicial, creacion README"
```
Con el comando ***git add {nombre del fichero}*** le decimos a Git que vamos a preparar un commit para ese archivo, si tenemos varios, lo haremos para cada archivo o en caso de que todos los que hemos modificado queremos commitearlos usaremos el comando ***git add -A***.

Con el comando ***git commit -m "{titulo del commit}"*** Haremos el commit con el mensaje entre comillas.

Finalizado el commit, haremos click en ***Publish Repository*** en **GitHub Desktop** para que de este modo llegue a **GitHub**.
