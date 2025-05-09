# **Clase 3**
## **Fusionamos una rama**
Usualmete fusionamos una rama para que los cambios que realizamos en una rama se incorporen o asimilen a otra rama, esto no siempre pasa por que hay ramas que tienden a quear en el olvido.

Para fusionar una rama debemos usar el comando:

- **git merge**
  
Al realizar este comando se realiza automaticamente un commit que nos incluye todos los cambios de la rama de origen a la rama en la que nos encontramos en ese momento. Si queremos editar o evitar que git haga el commit automaticamente usamos los siguientes comandos:

- **git merge --edit** (Abre el editor antes de hacer el commit)
- **git merge --no-commit** ( No hace el commit automaticamente)

## **Eliminar una rama**
Eliminar una rama es conciderado una buena practica, ya que hay muchas ramas que pueden perder funcionalidad a medida que nuestor proyecto vaya evolucionando.

Para eliminar una rama ejecutamos los siguiente comandos:

- git branch --delete nombre_de_la_rama
- git branch -d nombre_de_la_rama
  
## **Conflictos en git**
Se dan cuando git no es capaz de determinar que cambio es el que debe prevalecer una vez ocurra la fusión.

**¿Como los resolvemos?**

Cuando nos ocurra esto debemos seleccionar con que cambio nos quedaremos, si con los cambios de la rama main o nos quedamos con la rama chages.

