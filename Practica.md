# Etiquetar commits y ver diferencias

## 1. Etiquetar los commits 1 y 3

Primero visualizamos los commits que tiene nuestro repositorio actualmente: 

![](log%20oneline%20all.png)

Y a continuación con el siguiente comando etiquetaremos el commit: 

~~~
git tag -a etiqueta -m "commit" dir_commit
~~~

![](tag%20v1%20v3.png)

De esta forma el commit Version1 y Version3 tienen las etiquetas v1 y v3 respectivamente.

![](etiquetas.png)

Si queremos eliminar una etiqueta, utilizamos el siguiente comando:

~~~
git tag -d nombre_etiqueta
~~~

## Movernos entre etiquetas

Las etiquetas nos facilitan movernos entre los distintos commits ya que si asignamos un nombre significativo a un commit es más fácil saber a que commit estamos desplazándonos que si usamos la dirección de los commits.

Por ejemplo: 

![](checkout%20v3.png)

## Ver cambios de los commits

Si queremos ver los cambios que se han introducido en el repositorio, ejecutaremos el siguiente comando:

~~~
git show
~~~

Y el resultado en mi caso será el siguiente:

![](show.png)

## Diferencias entre commits

También podemos ver las diferencias entre dos commits, utilizando el commando: 

~~~
git diff etiqueta2..etiqueta2
~~~

Por ejemplo: 

![](diff.png)

La diferencia entre git show y git diff es que show te muestra los cambios que han habido en el commit que le indiques, mientras que el diff te muestra las diferencias entre dos commits distintos.
