# **Cursos de Git/Github**
## **¿Que es un control de versiones?**
Es un sistema que registra cada cambio que realices en el codigo funte de un proyecto. 
Esto nos permite tener un historial de cada uno de los cambios que se realizo y por quien se realizó el cambio. Una forma fácil de verlo es como marcar un checkpoint en un videojuego.

</p align="center"> <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSNKDkr_xT3R80sYfQOzWgqYfI-AX4w3Krqpg&s" alt= "branch" width="505" /> </p>

## **Importancia de un control de versiones**
Al usar un control de versiones tenemos beneficios como ser:
- **Colaboracion eficiente.** Permite que múltiples personas puedan trabajr en el mismo proyecto sin afectar al trabajo de otros, esto es gracias a las ramas.
- **Historial de cambios.** Nos permite ver que tipos de cambio se realizaron, cuándo y por quién se realizaron.
- **Seguridad y respaldo.** Brida una copia de seguridad de los archivos, lo que nos asegura la conservacion e integrida de los mismos.
- **Flexibilidad.** No es necesario un desarrollo lineal.

## **¿Que es git?**
Git es un sistema de control de versiones distribuida, que nos proporciona una copia del respositorio en nustra maquina local para despues pueda ser subido a un repositorio remoto, esto nos permite hacer trabajo colaborativo sin afectar al resto de participantes.

<img src= "https://www.azulschool.net/wp-content/uploads/2022/04/Flujo-de-trabajo-utilizando-Git-y-github-1024x867.jpeg" width= 300 align= "center"> 

## **¿Que es un repositorio?**  
 Es una carpeta donde se guardan las diferentes versiones de los ficheros de un proyecto, realiza un historial de cada cambio realizado. 
 Una forma facil de ver un repositorio es como una estanteria de libros o una estanteria en donde guardamos cajas con documentos con fecha y hora.

 ## **Iniciar un proyecto en git**
 Para iniciar un proyecto en git tenemos dos opciones, desde cero o uno ya excistente.
 - **Desde cero.** 
    1. **git init** < nombre de tu proyecto >
    2. **cd**< nombre del proyecto > 
- **Ya existente:**
  
    1. **cd** < directorio ya existente >
    2. **git init**
   
# **Clase 2**
## **Los 3 estados de git**
En Git excisten 3 estados, estos son:
- ### **Modified.** 
  Decimos que un archivo esta en un estado modified, cuando el archivo esta recien creado, eliminado o no tiene cambios registrados.
- ### **Staged.**
  Un archivo se encuentra en estado Staged, cuando el archivo a sido marcado como preparado para ser confirmado en el repositorio local.
- ### **Commited**
  Es cuando el archivo ya se encuentra guardad en el repositorio local.

  ## **Cambios de estado**
    Una vez creado el archivo, estamos en estado **modified** y para sar al estado de **Staged**, se debe seguir los siguientes pasos:

- **git status** (estado de git)
  
  ![Ejemplo status](./ejemploreadmemodified.png)
