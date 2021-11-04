# MANIPULACIÓN DE REPOSITORIOS EN GIT
## 1.1 CONFIGURACIÓN

<p align="justify">Una vez vista la instalación de Git, se podrá configurar este por medio del comando “git config” seguido de lo que se desea configurar. En este caso utilizaremos el siguiente comando para el nombre , e.mail y la activación del coloreado de salida:</p>

**<p align="center">git config --global user.name "Your-Full-Name"</p>**

**<p align="center">  git config --global user.email "your-email-address"</p>**

**<p align="center">  git config --global color.ui auto</p>**

**<p align="center">  git config --list</p>**

<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/55709ec32c1f5cef9cdb467a072112b197b96a02/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/1.png" title="Figura 1"></p>

## 1.2 CREACIÓN DE UN REPOSITORIO

<p align="justify">Ahora bien , para la creación de un repositorio será tan sencillo como utilizar el siguiente comando , siendo “dpl” el nombre del repositorio que se desea crear:</p>

**<p align="center">mkdir dpl</p>**

**<p align="center"> cd dpl</p>**

**<p align="center"> git init</p>**

**<p align="center"> ls -la</p>**

<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/55709ec32c1f5cef9cdb467a072112b197b96a02/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/2.png" title="Figura 2"></p>

## 1.3 COMPROBAR EL ESTADO DEL REPOSITORIO

<p align="justify">Para comprobar el estado del repositorio que se ha creado utilizaremos el comando:</p>

**<p align="center"> git status</p>**

<p align="justify">Una vez hecho esto crearemos un fichero indice.txt que contendrá :</p>

- Capítulo 1: Instalación de Git por el alumno XXX (donde XXX es el nombre del alumno)

- Capítulo 2: Flujo de trabajo básico

<p align="justify">Para ello introduciremos el siguiente comando:</p>

**<p align="center">cat > indice.txt</p>**

**<p align="center">*Ctrl+D* → Para cerrar</p>**

<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/55709ec32c1f5cef9cdb467a072112b197b96a02/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/3.png" title="Figura 3"></p>


<p align="justify">Hecho esto comprobaremos nuevamente el estado del repositorio, añadiremos el indice.txt y se volverá a comprobar el estado. Para añadir el indice.txt:
</p>

**<p align="center">git add indice.txt</p>**

<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/55709ec32c1f5cef9cdb467a072112b197b96a02/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/4.png" title="Figura 4"></p>


## 1.4 REALIZAR COMMIT'S

<p align="justify">En este caso se realizará un commit con el siguiente mensaje y se comprobará el estado nuevamente:</p>

**<p align="center">git commit -m "Añadido índice de la asignatura DPL."</p>**


<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/55709ec32c1f5cef9cdb467a072112b197b96a02/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/5.png" title="Figura 5"></p>

## 1.5 MODIFICACIÓN DE FICHEROS

<p align="justify">En este ejercicio se modificará el fichero indice.txt añadiendo dos capítulos más. Una vez hecho esto se mostrarán los cambios realizados con respecto a la versión anterior del repositorio, se añadirá el índice y por último se incluirá un commit:</p>

**<p align="center">cat > indice.txt</p>**

<p>Capítulo 1: Instalación de Git por el alumno XXX _(donde XXX es el nombre del alumno)_</p>
<p>Capítulo 2: Flujo de trabajo básico</p>
<p>Capítulo 3: Gestión de ramas</p>
<p>Capítulo 4: Repositorios remotos</p>


**<p align="center">*Ctrl+D* → Para cerrar</p>**

**<p align="center">git diff</p>**

**<p align="center">git add indice.txt</p>**

**<p align="center">git commit -m "Añadido los capítulos 3 y 4"</p>**

<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/55709ec32c1f5cef9cdb467a072112b197b96a02/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/6.png" title="Figura 6"></p>

## 1.6 HISTORIAL

<p align="justify">En cuanto al historial se refiere, podremos visionar la última versión del repositorio con respecto a la anterior:
</p>

**<p align="center">git show</p>**

<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/55709ec32c1f5cef9cdb467a072112b197b96a02/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/7.png" title="Figura 7"></p>

<p align="justify">Por último se introducirá un commit donde se especifique que se ha añadido un capítulo, y se volverá a mostrar nuevamente los cambios del repositorio:</p>

**<p align="center">git commit --amend -m "Añadido el capitulo sobre gestión de ramas al índice."</p>**


<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/55709ec32c1f5cef9cdb467a072112b197b96a02/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/8.png" title="Figura 8"></p>
