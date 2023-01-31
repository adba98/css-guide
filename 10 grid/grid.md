# Grid

Modelo de layout que permite construir cuadrículas dinámicas

- display: grid (inline-grid)
- Necesita un contenedor (grid-container) y al menos un hijo (grid-item)
- Los items serían las celas de la cuadrícula (contenedor)

# Términos

- Grid column: Cada columna de la cuadrícula
- Grid row: Cada fila de la cuadrícula
- Grid cell: Cada celda de la cuadrícula
- Grid gap: Separación entre celdas
- Grid line: Líneas que delimitan cada columna/fila
- Span: establece el número de columnas o filas que debe ocupar

# Ventajas

- Cada celda es dinámica (la cuadrícula se adapta)
- Podemos decir cuando empieza o acaba la columna

# Propiedades:

- `grid-template-rows` Tamaño de las filas
- `grid-template-columns` Tamaño de las columnas
- `row-gap` Separación entre filas
- `column-gap` Separación entre columnas
- `grid-row-start` Establece desde que row-line empezara el elemento
- `grid-row-end` Establece hasta que row-line llega elemento
- `grid-column-start` Establece desde que column-line empezara el elemento
- `grid-column-end` Establece hasta que column-line llega el elemento

\* start y end: Admite valores positivos, negativos y span

- Positivos: Cuenta las líneas de izquierda a derecha
- Negativos: Cuenta las líneas de derecha a izquierda
- `span`: Establece cuantas columnas ocupa

Tip: end en -1 hace que llegue a final

## Medidas adicionales para grid

- fr: Equivale a `n` fracciones del espacio disponible, después de establecer medidas fijas
- auto: Equivale al espacio que quede después de repartir todos los elementos
- Función repeat(): establece la repetición de medidas o patrones

# Explicit y Implicit grid

El explicit grid es aquel que se declara y el implicit son aquellos valores que quedan por fuera del explicit grid

- `grid-auto-columns` Establece que hacer con las columnas no definidas
- `grid-auto-rows` Establece que hacer con las filas no definidas
- `grid-auto-flow` Establece la dirección en la cual se va a pintar el implicit grid + `dense`

# Alineamiento

- justify-items
- align-items
- align-content
- justify-content
- justify-self
- align-self
- order

# Grid Areas

## Otros

- `minmax()`: Recibe 2 parámetros que establecen el mínimo y el máximo que pueden tener los ítems
- min-content: Mínimo necesario en función del contenido
- max-content: Máximo necesario en función del contenido
- auto-fill: Crea tantos grid-iems como le permita el viewport (respetando las medidas)
- auto-fit: Elimina los grid-items vacíos que no se estén ocupando

# Shorthand

- `gap: row-gap column-gap`
- `grid-column`: start `/` end
- `grid-row`: start `/` end
- `place-items: align-items justify-items`
- `place-content: align-content justify-content`
- `place-self: align-self justify-self`
