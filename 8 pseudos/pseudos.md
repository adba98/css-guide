# Pseudo elementos

- Sirven para dar estilos a partes específicas de un elemento
- Sintaxis `selector::pseudo-element`

Tipos:

- `first-line`: Para elementos de bloque. Sirve para seleccionar primera línea
- `first-letter`: Para elementos de bloque. Sirve para seleccionar primera letra
- `selection`: Retirado de la especificación, da estilos a la selección del contenido

Los dos siguientes tipos necesitan de la propiedad `content`, son elementos de línea por defecto y se vuelven hijos del elemento al que pertenecen.

- `before`
- `after`

# Pseudo clases

Selectores que reaccionan en tiempo real, de acuerdo a la interacción del usuario con los elementos

- Funcionan con todos los selectores de CSS
- No están atados a ningún elemento
- Sintaxis `selector:pseudo-class` o `:pseudo-class`
