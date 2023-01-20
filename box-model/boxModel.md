# Box Model

La web se compone de cajas, y estas cajas tiene las siguientes propiedades:
- Contenido: texto, imagen, etc.
- Borde
- Padding: Distancia entre el contenido y borde de la caja
- Margin: Distancia entre una caja con las que le rodea
- Ancho
- Alto

Tipos de elementos:
* De bloque
* De línea: El tamaño lo determina el contenido

## Margin y Padding:
* Los elementos en línea solo tienen margen horizontal
* El padding funciona igual para ambos tipos de elemento

Recomendaciones:
* No usar márgenes en el selector universal (*) si no es necesario
* No afectar todos los márgenes si no es necesario con la propiedad ``margin``
* No colocar margin al body
* Los márgenes verticales colapsan, por lo que es recomendable usar ``margin-bottom``

## Border
La propiedad ``border`` **modifica** las propiedades que por defecto ya tenía

## Box sizing
Box sizing es la propiedad que nos permite controlar el cálculo que hace el navegador a la hora de modificar las propiedades ``content``, ``padding`` y ``border``.

* ``border-box``: valor que calcula el tamaño del elemento, incluyendo el ``padding`` y el``border``