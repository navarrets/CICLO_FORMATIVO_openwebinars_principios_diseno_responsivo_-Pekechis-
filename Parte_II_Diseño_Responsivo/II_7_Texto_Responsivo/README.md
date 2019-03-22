## II.8 Texto Responsivo

Cuando hablamos de diseño responsivo solemos dar más importancia al layout, pero el texto que vamos a presentar es igual de importante para conseguir un buen diseño.

Si no tenemos cuidado nos podemos en contrar con varios problemas:

- Líneas cortas con pocos caracteres, lo que dificultan la lectura.
- Líneas largas con muchas caracteres, lo que también dificulta la lectura.
- Caracteres muy pequeños.

Lo ideal, según estudios, es una letra de un tamaño adecuado, para poder leer sin forzar la vista, y que se disponga formando líneas de entre 60-80 caracteres.

Para intentar solucionar esto con garantías lo más recomendable es utilizar para el texto unidades de tamaño relativas al viewport. Tendremos:

- **vw** en relación a la anchura del viewport.
- **vh** en relación a la altura del viewport.
- **vmin** el valor menor en relación a la dimensión pequeña del viewport (anchura o altura).
- **vmax** el valor máximo en relación a la dimensión más grande del viewport (anchura o altura).

Teniendo en cuenta, por ejemplificar que 1vw es un 1% de la anchura del viewport.

No obstante encontrar siempre el tamaño perfecto de texto es algo que puede ser complicado sino imposible. Sin embargo allí van unas posibles pautas:

- Calcular el tamaño mínimo y máximo que me puedo permitir usando calc() (función css)
- No importa si el texto hace "reflow" (pasa a la siguiente línea) en determinadas ocasiones.
- Mantener el tamaño perfecto de línea puede que sea imposible.
- Si tenemos que elegir es conveniente priorizar móviles y tablets.
- En algunos elementos, por ejemplo en un menú de navegación, puede tener sentido usar tamaño fijos de letra en vez de unidades relativas al viewport.

Curso desarrollado por [pekechis](http://github.com/pekechis) para [OpenWebinars](https://openwebinars.net/)
