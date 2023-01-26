# FlexBox

Es un modelo de **Layout** el cual posee algoritmos que define como los elementos serán presentados en pantalla, permite flexibilidad en las cajas

Creado por necesidad y mal uso de propiedades como: table, float, position

- Diseños Flexibles con menos código
- Maneja un eje vertical (V) y horizontal (H)
- Manejar el orden de los elementos
- Definir orientación de los elementos
- Definir tamaños flexibles en las cajas
- Requiere de una relación padre e hijo(s)
- Maneja dos ejes por defecto
  - Main Axis
  - Cross Axis

# Propiedades

- display: Define el contexto de un contenedor flexible (flex, inline-flex)
- flex-direction: Establece la dirección del eje principal (row, colum, row-reverse, colum-reverse)
- flex-wrap: Permite ajustar los elementos en diferentes líneas (nowrap, wrap, wrap-revese)

## Alineación

- justify-content: Alinea elementos en el eje principal.
  (space-evenly, flex-start, flex-end, center, space-around, space-between)
- align-items: Alinea en el eje secundario para una sola línea de elementos (stretch, flex-start, flex-end, center)
- align-content: Alinea en el eje secundario (multilínea)
- align-self: Alinear elemento específico (hijos)

## Secundarias

- flex-basis: Tamaño base del ítem (remplaza el `width`)
- flex-grow: Establece los tamaños de acuerdo al espacio sobrante
- flex-shrink: Establece los tamaños cuando no falta espacio
- order: Establecer el orden (valor) que ocupara en el contenedor

# Valores

- flex-start: Los artículos se colocan al principio del contenedor
- flex-end: Los artículos se colocan al final del contenedor
- center: Los artículos se colocan en el centro del contenedor
- space-between: Los artículos tendrán espacio entre ellos
- space-around: Los elementos tendrán espacio antes, entre ellos y después de ellos
- space-evenly: Los artículos tendrán el mismo espacio a su alrededor

# Shorthands

- flex-flow: flex-direction flex-wrap
- flex: Grow Shrink Basis
