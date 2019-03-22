# II.6 Tablas Responsivas

Las tablas son un elemento problemático a la hora de realizar **Diseño Responsivo** ya que en cuanto tienen un número de columnas considerable pueden provocar la aparición del tan temido _scroll horizontal_ en nuestra página web, sobre todo en pantallas pequeñas.

Para afrontar este tipo de problemas hay tres soluciones que son aceptadas como buenas:

- Esconder columnas.
- Convertir las filas en listas
- Crear un scroll horizontal que solo se aplique a la tabla.

## Esconder columnas

Esta técnica consiste básicamente en esconder ciertas columnas, que debe de ser las menos importantes, cuando el tamaño de la pantalla es menor que un breakpoint establecido.

Tiene las siguiente ventajas:

- Conseguimos un diseño responsivo.
- Priorizo el contenido que quiero mostrar.

Aunque también tiene desventajas:

- Pierdo información en determinadas pantallas.

Un ejemplo para conseguir esto sería una hoja de estilos similar a esta:

```css
@media screen and (max-width: 576px) {
  .hidden td.primero,
  .hidden th.primero {
    display: none;
  }
}

@media screen and (max-width: 768px) {
  .hidden td.segundo,
  .hidden th.segundo {
    display: none;
  }
}
```

En ese diseño tenemos dos **_breakpoints_** y ocultaremos unas u otras columnas dependiendo del tamaño (la que tienen la clase _.primero_ la clase _.segundo_)

## Convertir Listas a filas

Esta técnica consiste en hacer desaparecer las cabeceras de la tabla cuando la pantalla es menor que una determinada cantidad y hacer que todas las celdas se conviertan en elementos de bloque para que se muestren una debajo de otra y no al lado.

Tiene las siguiente ventajas:

- Conseguimos un diseño responsivo.
- No pierdo información.

Aunque también tiene desventajas:

- No priorizo la información.
- "Desplazo" mucho el resto del layout hacia abajo.

## Scroll controlado

Esta técnica consiste en acotar el scroll horizontal para que si ha de aparecer solo afecte a la tabla y no a la página entera.

Tiene las siguiente ventajas:

- Conseguimos un diseño responsivo.
- No pierdo información.

Aunque también tiene desventajas:

- No priorizo la información.
- Aunque local sigue habien un scroll horizontal.

Para conseguir esto debemos "envolver" la tabla en un contenedor y darle las siguiente propiedades:

```html
<div class="localscroll">
  <table>
    .....
  </table>
</div>
```

```css
div.localscroll {
  overflow-x: auto;
  width: 100%;
}
```

No obstante no hay una solución universal. Debemos experimentar según el Layout que tengamos para ver cuál de estas técnicas (o la mezcla de ellas) se adecúa mejor a nuestro diseño.

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
