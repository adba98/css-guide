# Fundamentos CSS

## Sintaxis:

- Regla = selector + declaración(es)
- Declaración = Propiedad + valor

```css
selector {
  propiedad: valor;
  propiedad: valor;
}
```

## Especificidad

Establece que tan especifico es un selector para saber qué estilo aplicar.

La prioridad se da de acuerdo al siguiente cálculo:

- Etiquetas y pseudoelementos (0,0,1)
- Clases, atributos y pseudoclases (0,1,0)
- Ids (1,0,0)
- Estilos en línea (1,0,0,0)

**Nota:**

`!important` se sobrepone a cualquier especificidad (No es buena práctica usarlo)

**Ejemplo:**

El siguiente selector se compone de una etiqueta, una clase y un ID, por lo tanto, su especificidad es de `(1,1,1)`. En el caso de que sea igual la especificidad funciona la cascada

```css
h1.text#text {
}
```

> El grafico de [CSS Specificity Graph Generator][specificity] permite conocer que tan buen codigo estamos realizando

## Herencia

La herencia es la capacidad que tienen algunos elementos de heredar algunas propiedades de sus elementos contenedores. No todas las propiedades heredan.

- `inherit` permite herencia elementos que no lo son
- `initial` le quita la herencia a un elemento

## Prefijos propietarios

- ms (Microsoft System)
- webkit (Chrome)
- o (Opera)
- moz (Mozilla)

<!-- Markdown links -->

[specificity]: https://jonassebastianohlsson.com/specificity-graph/
