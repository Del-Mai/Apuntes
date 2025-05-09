# **Clase 3**
## **Fusionamos una rama**
Usualmete fusionamos una rama para que los cambios que realizamos en una rama se incorporen o asimilen a otra rama, esto no siempre pasa por que hay ramas que tienden a quear en el olvido.

Para fusionar una rama debemos usar el comando:

- **git merge**
  
Al realizar este comando se realiza automaticamente un commit que nos incluye todos los cambios de la rama de origen a la rama en la que nos encontramos en ese momento. Si queremos editar o evitar que git haga el commit automaticamente usamos los siguientes comandos:

- **git merge --edit** (Abre el editor antes de hacer el commit)
- **git merge --no-commit** ( No hace el commit automaticamente)
- 