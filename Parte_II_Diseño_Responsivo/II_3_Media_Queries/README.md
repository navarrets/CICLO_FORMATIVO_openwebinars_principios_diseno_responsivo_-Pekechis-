# II.3 Media Queries

Una de las herramientas esenciales para poder realizar un diseño responsivo de calidad son las **_media-queries_** que son:

> ...módulo de CSS3 que nos permite adaptar al representación del contenido a las características del dispositivo...

[Definición extraida de Wikipedia](https://es.wikipedia.org/wiki/Media_query)

## Síntaxis de las Media-Queries

Las media queries son expresiones en las que indicamos un tipo de medio y una consulta en relación a las características del dispositivo como alto, ancho e incluso color:

Algo similar a lo siguiente:

```css
@media mediatype [condiciones] {
  .... /* Estilos para esas condiciones */ ....;;
}
```

Los distintos tipos de valores que puedo tener para **_mediatype_** son:

- all
- screen (el más usado)
- tty (terminal)
- print (para impresoras)
- tv (para pantallas de televisión)
- projected (para proyectar contenidos)
- braille (para dispositivos para invidentes)
- etc...

En cuanto a las condiciones que puedo consultar:

- width | min-width | max-width
- height | min-height | max-height
- orientation (landscape / portrait)
- aspect-ratio | min-aspect-ratio | max-aspect-ratio
- color | min-color | max-color

Esta condiciones se pueden combinar y modificar utilizando claúsulas como:

- And
- Not
- All
- Only

Si juntamos todo podemos ver algunos ejemplos:

```css
/* Estilos para todo tipo de pantallas con una anchura máxima
de 576px*/
@media all and (max-width: 576px) {
  .....;
}

/* Estilos para pantallas con al menos 992px de anchura y que estén apaisadas (más ancho que alto)*/
@media screen and (min-width: 992px) and (orientation: landscape) {
  ......;
}

/* Estilos sólo para pantallas que tengan al menos 768px de anchura*/
@media only screen and (min-width: 768px) {
  ......;
}
```

## Hojas de estilos diferentes

Podemos usar media-queries en la etiqueta link para seleccionar hojas de estilos diferentes atendiendo a las cracterísticas del dispositivo.

Por ejemplo:

```html
<!--Para pantallas de hasta 576px de ancho -->
<link rel="stylesheet" media="(max-width: 576px)" href="small.css" />

<!--Para pantallas entre 576px y 768px de ancho -->
<link rel="stylesheet" media="(max-width: 768px)" href="medium.css" />

<!--Para pantallas entre 768px y 992pxde ancho -->
<link rel="stylesheet" media="(max-width: 992px)" href="large.css" />
```

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
