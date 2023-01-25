# Medidas

## Absolutas

No cambian y mantendrán su tamaño

- px
- cm, mm, Q, in, pc, pt

### rem vs. em

Ambas medidas se calculan con base en el `font-size` (tamaño de fuente)

- `rem`: Corresponde a la medida "m" de la raíz del documento
- `em`: Corresponde a la medida "m" del contexto en donde se encuentre

> Se usa el caracter `m` puesto que es el que mas espacio ocupa siempre

> Nota: El tamaño fuente de la raiz es de 16px se recomienda no modificar

## Relativas

Dependen de un **contexto**

- em, rem, %, vw, vh, vmin, vmax
- ex, ch, lh

## Width con % vs. width auto

- `%`: Se usa de referencia el tamaño del contenedor y el navegador calcula el porcentaje. Esto no ocurre cuando usamos `transform`
- `auto`: El navegador calcula según el espacio disponible

> Si aparecen scrolls innecesarios puede que necesites entender esto

## Height con % vs. height auto

- `%`: En un contenedor debe tiene el alto declarado, si no, no puede calcular el porcentaje y lo interpreta como un `auto`
- `auto`: Calculará el navegador con base en el contenido del elemento

### Viewport

Es el área útil en donde se muestra la página web (Área visible sin hacer scroll)
