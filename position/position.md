# Positon

Conceptos:

- Flujo de renderizado: Por norma general los elementos se dibujan de izq a der y de arriba hacia abajo
- Espacio reservado: Espacio asignado a elemento en el navegador
- Elemento posicionado: significa que el elemento tiene un valor diferente a `static` (default)
- Stackin context: Orden en el que se apilan las cajas que se superponen, dentro del mismo contenedor.

Propiedades:

- `top`: Moverá el elemento desde la parte superior
- `right`: Moverá el elemento desde la parte derecha
- `bottom`: Moverá el elemento desde la parte superior
- `left`: Moverá el elemento desde la parte izquierda
- `z-index`: Moverá el elemento en el contexto de apilamiento (eje Z)

> Nota: La propiedad `top` y `left` invalidan la propiiedad `bottom` y `right`

Valores:

- Static: No está posicionado (no se puede mover)

- Relative: Mantiene posición y medidas en el flujo de renderizado y mantendrá su espacio reservado. Si lo movemos, lo hará usando su posición en el HTML como punto de referencia.

- Absolute: Pierde medidas en el flujo de renderizado y su espacio reservado. Usa el elemento contenedor como referencia, si no tiene, usa el HTML

- Fixed: Igual que el absoluto, pero se posiciona siempre sobre el HTML. Al hacer scroll se queda fijo

- Sticky: Mezcla entre relative y “fixed”

## Stacking context

El contexto de apilamiento es el espacio en el cual los elementos se apilan adelante o por detrás de otros. El orden es (de adelante a atrás)

- Elementos posicionados con `z-index` ≥ 1
- Elementos posicionados sin `z-index` (auto)
- Elementos no posicionados
- Elementos posicionados con `z-index` ≤ 1
