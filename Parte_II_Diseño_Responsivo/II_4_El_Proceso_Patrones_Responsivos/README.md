# II.4 El proceso de diseño. Patrones responsivos.

Afrontar un proyecto que requiera el desarrollo de una página web responsiva no es fácil y hay varias estrategias posibles para afrontarlo. No obstante ya es comunmente aceptado que lo más recomendable es lo siguiente:

![Start Small](img/small.png)

Es decir, que el proceso de diseño de nuestra página web debe empezar haciendo que todo quede correctamente en pantallas pequeñas. De este manera:

- **Priorizo** siempre lo que es importante. Si el proceso fuera al revés es muy fácil que caigamos en el error de quitar cosas que sean realmente importantes.
- Me pregunto en cada diseño si es **necesario un diseño nuevo** para paltallas más grandes.
- Elijo los **breakpoints** más adecuados.

## Patrones Responsivos

En nuestro proceso de diseñar web responsivas debemos conocer lo que se conoce como **_patrones responsivos_**.

Los **_patrones responsivos_** son soluciones que se han dado por buenas para el problema de diseñar páginas web responsivas. Hay muchos pero los más comunes son lo siguientes:

- Column Drop
- Mostly Fluid
- Layout Shifter
- Off Canvas
- ...
- Mezclar varios de ellos
- Pequeños ajustes (Tiny Tweaks)

A continuación pasamos a comentar los principales, los cuatro primeros para los que hay un ejemplo en esta misma carpeta de este repositorio:

### Column Drop

Es el patrón más básico y consiste en que en cada breakpoint se va a apilando un elemento

### Mostly Fluid

Parecido a Column Drop. Es una cuadrícula fluida y en cada breakpoint hay redimensionamiento de varias columnas.

### Layout Shifter

Es el patrón más responsivo, en cada breakpoints cambia el diseño del layout, no únicamente el flujo y la anchura de los elementos.

### Off Canvas

En vez de apilar contenidos éstos se colocan fuera de la pantalla cuando el tamaño de pantalla no es lo suficientemente grande.

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
