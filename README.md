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
  
  Una vez ya ejecutes los comandos saldria algo como:

![](imagenes/Ejemploreadmemodified.png)

Para ejemplo llevaremos a **saged** el archivo Ejemploreadme.md:
- **git add** Ejemploreadme.md
  
  Nuestro archivo esta listo para ser agregado 
- **git commit** se abrira una ventana en VS

Guardas el archivo y lo cierras, tu comit ya estaria hecho.
## **¿Que es un comit?**
Podemos verlo como como un checkpoint en un videojuego, a medida que vamos avanzando tenemos puntos de guardado que resguardan tu progreso en el juego, al tener estos checkpoints puedes volver a cualquiera de estos cuando lo desees ya que estan en un registro de los avances que tuviste.

Un **commit** es similar nos permite registrar los cambios hecho en un repositorio asi tambien cuando y por quien fueron realizados.

## **¿Como hacemos un commit?**
Para hacer un commit los archivos deben haber estado previamente en la etapa de Staged.
Para guardar los cambios hechos puedes usar el sguiente comando:

- **git commit -m "titulo del commit"**

Esto creará un nuevo commit en tu repositorio y añadirá una referencia al commit en la rama que estes trabajando.

El mensaje de commit que se esncuentra entre comillas se usa como titulo del comit donde se describe los cambios realizados.

## **¿Que es el HEAD?**
El HEAD es un marcador que te indica en que commit te encuentras actualmente.

En pocas palabras te dice "estas aquí", y puedes verlo con el siguiente comando:
 
- **git log**

Ejemplo:

![](imagenes/ejemplogitlog.png)

Para ejemplo llevaremos a **saged** el archivo Ejemploreadme.md:
- **git add** Ejemploreadme.md
  
  Nuestro archivo esta listo para ser agregado 
- **git commit** se abrira una ventana en VS

Guardas el archivo y lo cierras, tu comit ya estaria hecho.
## **¿Que es un comit?**
Podemos verlo como como un checkpoint en un videojuego, a medida que vamos avanzando tenemos puntos de guardado que resguardan tu progreso en el juego, al tener estos checkpoints puedes volver a cualquiera de estos cuando lo desees ya que estan en un registro de los avances que tuviste.

Un **commit** es similar nos permite registrar los cambios hecho en un repositorio asi tambien cuando y por quien fueron realizados.

## **¿Como hacemos un commit?**
Para hacer un commit los archivos deben haber estado previamente en la etapa de Staged.
Para guardar los cambios hechos puedes usar el sguiente comando:

- **git commit -m "titulo del commit"**

Esto creará un nuevo commit en tu repositorio y añadirá una referencia al commit en la rama que estes trabajando.

El mensaje de commit que se esncuentra entre comillas se usa como titulo del comit donde se describe los cambios realizados.

## **¿Que es el HEAD?**
El HEAD es un marcador que te indica en que commit te encuentras actualmente.

En pocas palabras te dice "estas aquí", y puedes verlo con el siguiente comando:
 
- **git log**

Ejemplo:

![](imagenes/ejemplogitlog.png)

## **¿Que es una rama?**

Una rama es una linea de desarrollo independiente o una version de el repositorio. al ser una bifurcacion de nuestra rama principal nos permite relizar cambios manteniendolos en esa rama y separandolas de los demas, esto hace posible el desarrollo en paralelo sin afectar a las demas ramas o a la rama principal.

Debemos tomar en cuenta que cuando vallamos a realizar cambios por mas pequeños que sean se debe crea una rama para asi encapsular dichos cambios, estos cambios tambien se podran unir a la rama principal una vez el trabajo este realizado.

![](imagenes/ramas.png)

## **¿Como creamos una rama?**
 Para la creacion de una rama debemos realizar el siguiente comando:
 
 - **git branch rama_nombre de la rama**
  
Esto nos generara una rama mas no nos cambia de rama. 
## **¿Entonces como cambiamos de rama?**
 Para cambiar de rama tenemos 2 opciones de comando:

 - **git checkout rama_nombre de la rama**
 - **git switch rama_nombre de la rama**
  
  De estas dos opciones la se recomienda el uso de git switch, ya que git checkout tiene mas funciones además de cambiar de rama. Tambien es recomendable que despues del cambio de rama se realice un git log para que te muestre el HEAD y así asegurarse de que estás en la rama que deses.

# **Clase 3**
## **Fusionamos una rama**
Usualmete fusionamos una rama para que los cambios que realizamos en una rama se incorporen o asimilen a otra rama, esto no siempre pasa por que hay ramas que tienden a quear en el olvido.

Para fusionar una rama debemos usar el comando:

- **git merge**
  
Al realizar este comando se realiza automaticamente un commit que nos incluye todos los cambios de la rama de origen a la rama en la que nos encontramos en ese momento. Si queremos editar o evitar que git haga el commit automaticamente usamos los siguientes comandos:

- **git merge --edit** (Abre el editor antes de hacer el commit)
- **git merge --no-commit** ( No hace el commit automaticamente)
