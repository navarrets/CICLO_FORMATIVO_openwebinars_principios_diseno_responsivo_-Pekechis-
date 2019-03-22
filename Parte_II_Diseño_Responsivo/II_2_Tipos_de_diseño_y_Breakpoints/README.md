# II.2 Tipos de diseños y Breakpoints

En el apartado anterior hemos conocido el importante concepto del **_Viewport_** y ahora, antes de lanzarnos a hacer diseño responsivo vamos a continuar introduciendo los diferentes tipos de diseños o layouts que podemos tener.

Hay clasificaciones más complejas pero si condensamos podemos establecer que hay tres tipos de diseños o layouts a la hora de hacer maquetación web.

- **Fixed:** Donde la anchura de la página es fija y es expresada en pixels.
- **Elastic:** Donde la anchura de la página es fija y es expresada en la unidad **em** (múltiplos del tamaño de letra).
- **Fluid/Liquid/Relative:** Donde la anchura de la página depende del tamaño del Viewport del usuario y se expresa en porcentajes (%).

A continuación vamos a explicar de manera concisa las ventajas y desventajas de cada uno de estos tipos.

## Fixed Layout

**Ventajas:** Tenemos un control total sobre el layout ya que especificamos dimensiones fijas.

**Desventaja:** Puede aparecer un scroll horizontal en pantallas pequeñas (si no escalo).

Sin embargo, este tipo de Layouts puede tener sentido si no quiero cambiar nunca el layout ni sus proporciones en ningún dispositivo (no suele ser el caso para las pantallas de los móviles).

## Elastic Layout

**Ventajas:** Control al hacer zoom-in y zoom-out. Se mantienen las proporciones.

**Desventajas:**

- Al final es igual que fixed.
- Es difícil calcular las dimensiones reales.
- Ems se calcula en relación al padre, podemos necesitar rems.
- No hay fluidez cuando cambia el tamaño de pantalla. No se adapta bien.

## Fluid Layout

**Ventaja:** Se adapta al Viewport, al tamaño de lo que está viendo el usuario.

**ES EL TIPO DE LAYOUT QUE SE USA PARA DISEÑO RESPONSIVO**

## Breakpoints

Una vez hemos establecido que usaremos diseños de tipo **_Fluid_** debemos recordar que el concepto de diseño responsivo, además de **_adaptación_** al tamaño implicaba el **_cambio_** en el diseño atendiendo al tamaño u otras características del dispostivo.

La anchura de la pantalla en la que se produce el cambio es lo que se conoce como **_Breakpoint_**.

La elección de unos **_breakpoints_** adecuados no es una tarea fácil pero tenemos la suerte de que ya ha habido empresas que han hecho estudios muy serios al respecto. Destacar los Breakpoints elegidos por [Twitter BootStrap](https://getbootstrap.com/):

- <576px (pantallas pequeñas)
- 576px-768px (móviles apaisados)
- 768px-992px (tablets)
- 992px-120ppx (desktop)
- \>1200px (pantallas grandes)

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
