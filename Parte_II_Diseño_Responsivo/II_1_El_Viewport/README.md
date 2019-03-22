## II.1 El Viewport

Uno de los concepto más importantes que debemos conocer antes de lanzarnos a realizar diseños responsivos es el concepto de **_Viewport_**.

Una posible definición sería:

_Área de la pantalla en la que el navegador puede renderizar contenido, es decir, el espacio disponible para mostrar mi página web._

Este concepto es muy fácil de comprender cuando nos referimos a él en sistemas de escritorios o en laptops o portátiles. En estos casos el **Viewport** coincide con la pantalla de nuestro navegador.

![Viewport en Sistemas Desktop/Laptop](img/viewport_desktop.png)

Sin embargo, si nos referimos a móviles y tablets estaremos hablando de otra cosa diferente.

Cuando este tipo de dispositivos irrumpieron la páginas se maquetaban usando normalmente una anchura fija en píxels que solía variar entre 800px y 1000px que, obviamente, era mayor que la anchura de la pantalla de los móviles.

Ante esta circunstancia los fabricantes hicieron que este tipo de dispositivos tuvieran dos **Viewports**:

- El **_Layout-viewport_** que es el viewport que es tenido en cuenta para la aplicación de estilos.Suele ser de aproximadamente 900px.
- El **_Visual-viewport_** que es el viewport que realmente ve el usuario cuando está navegando.

![Viewport en Sistemas Mobile](img/mobile_viewport.png)

Además, sucede que en este tipo de dispositivos podemos hacer Zoom mediante gestos lo que provoca que:

- No cambie el **_Layout-viewport_**
- Cambie el **_Visual-viewport_**.

Y no acaban ahí los problemas. También, en este mundo de miles de dispositivos diferentes no vamos a encontrar con que tenemos que lidiar con diferentes valores para los:

- **Hardware Pixels:** que son los pixels de resolución que nos da la tarjeta gráfica.
- **DPI(Device Independent Pixels):** Que es la unidad de medida del navegador. Se relaciona con la distancia real y ocupan lo mismo independientemente de la densidad de pixels de la pantalla.
- **DPR(Device Pixel Ratio):** Hw Pixel / DPI (es una dimensión)

Esto, todo junto, es un jaleo y hay multitud de teoría detrás. Sin embargo, lo que necesitamos para empezar a gestionar toda esta situación es simplemente añadir una línea en la cabecera de mi página Web.

```html
<head>
  ...
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  ...
</head>
```

Con esa simple línea podremos empezar a maquetar diseños responsivos de manera eficifiente e incluso hraremos que las páginas que no están preparadas para móviles se muestren correctamente aunque tengamos, eso sí, que hacer continuos **_zooms_** para poder usarlas.

Si estáis interesados en profundizar más hay un vídeo muy interesante y aclaratorio (de 44min) sobre el **_Viewport_**.

[Enlace al vídeo](https://vimeo.com/52851511).

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
