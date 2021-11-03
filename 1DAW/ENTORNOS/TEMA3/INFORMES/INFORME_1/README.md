# INSTALACION DE GIT

<div align="justify">

Existen dos maneras para instalar Git en nuestro equipo:

- Con paquetes predeterminados
- Desde la fuente

No obstante en este informe se hará mención al primero de ellos.

Para la instalación de Git por medio de paquetes predeterminados será necesario comprobar previamente si el equipo no cuenta ya con una versión de Git. Para ello se utilizará el comando:
<div align="justify">

**<p align="center"> git --version </p>**

<p align="center"><img src="https://github.com/jdabrante/CLASES/blob/d1d14b98d80b6af1f3a14e5b56817a7a59fc61ba/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/GIT.1.png" title="Figura 1"></p>
  
<p align="justify">Como se puede observar en la figura 1, el equipo no cuenta con ninguna versión de Git instalada, por lo que se procederá a la instalación de la  misma.</p> 
<p align="justify">A continuación , para la instalación se debe actualizar el índice de paquetes y, posteriormente, se iniciará la instalación, todo ello a través de los respectivos comandos (Fig.2 y Fig.3):</p>

  **<p align="center">sudo apt update</p>**
  **<p align="center">sudo apt install git</p>**
  
  <p align="center"><img src="https://github.com/jdabrante/CLASES/blob/d1d14b98d80b6af1f3a14e5b56817a7a59fc61ba/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/GIT.2.png" title="Figura 2"></p>
  
  <p align="center"><img src="https://github.com/jdabrante/CLASES/blob/d1d14b98d80b6af1f3a14e5b56817a7a59fc61ba/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/GIT.3.png" title="Figura 3"></p>
  
Una vez hecho esto se comprobará la versión instalada:
  
  **<p align="center">git --version</p>**
 
 <p align="justify">Así pues, y como bien se observa en la figura 4, la versión instalada por medio de este método se trata de la 2.25.1.</p>
  
   <p align="center"><img src="https://github.com/jdabrante/CLASES/blob/d1d14b98d80b6af1f3a14e5b56817a7a59fc61ba/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/GIT.4.png" title="Figura4"></p>
  
  

## CONFIGURACION DE GIT
  
  <p align="justify">Terminada la instalación , a continuación se procederá a la configuración de Git. Esto es necesario ya que los mensajes de confirmación deberán de generar información correcta para así verificar una buena praxis a medida que el proyecto es compilado.</p>
  
  Para ello utilizaremos el comando:

  **<p align="center">git config --global user.name “Nombre”</p>**
  **<p align="center">git config --global user.email "Correo del usuario"</p>**
  
  <p align="justify">Estos parámetros serán necesarios, ya que Git insertará esta misma información en cada confirmación que se haga. Para comprobar los elementos de configuración se utilizará el siguiente comando, que nos mostrará los datos introducidos en el comando anterior como se observa en la figura 5:</p>
  
  **<p align="center">git config --list</p>**
  
  <p align="center"><img src="https://github.com/jdabrante/CLASES/blob/d1d14b98d80b6af1f3a14e5b56817a7a59fc61ba/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/GIT.5.png" title="Figura5"></p>
  
  <p align="justify">Por último, si se quisiera modificar la información almacenada en el archivo de configuración de Git se podrá bien editar manualmente o a través del comando:</p>
  
  **<p align="center">nano ~/.gitconfig</p>**
  
  <p align="justify">Una vez introducido este comando se nos mostrará una ventana con la información del archivo de configuración editable.</p>
  
  <p align="center"><img src="https://github.com/jdabrante/CLASES/blob/d1d14b98d80b6af1f3a14e5b56817a7a59fc61ba/1DAW/ENTORNOS/TEMA3/INFORMES/IMAGENES/GIT.6.png" title="Figura6"></p>
  
