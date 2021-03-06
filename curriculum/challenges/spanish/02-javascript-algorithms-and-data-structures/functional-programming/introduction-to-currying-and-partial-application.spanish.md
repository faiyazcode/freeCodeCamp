---
id: 587d7dab367417b2b2512b70
title: Introduction to Currying and Partial Application
challengeType: 1
videoUrl: ''
localeTitle: Introducción al curry y aplicación parcial.
---

## Description
<section id="description"> La <code>arity</code> de una función es el número de argumentos que requiere. <code>Currying</code> una función significa convertir una función de N <code>arity</code> en N funciones de <code>arity</code> 1. En otras palabras, reestructura una función para que tome un argumento, luego devuelva otra función que tome el siguiente argumento, y así sucesivamente. Aquí hay un ejemplo: <blockquote> // Función sin currículum <br> función unCurried (x, y) { <br> devuelve x + y; <br> } <br><br> // Función de curry <br> función curry (x) { <br> función de retorno (y) { <br> devuelve x + y; <br> } <br> } <br> Curried (1) (2) // Devoluciones 3 </blockquote> Esto es útil en su programa si no puede suministrar todos los argumentos a una función al mismo tiempo. Puede guardar cada llamada de función en una variable, que mantendrá la referencia de función devuelta que toma el siguiente argumento cuando esté disponible. Aquí hay un ejemplo que usa la función de <code>curried</code> en el ejemplo anterior: <blockquote> // Llamar una función al curry en partes: <br> var funcForY = al curry (1); <br> console.log (funcForY (2)); // Impresiones 3 </blockquote> De manera similar, <code>partial application</code> puede describirse como la aplicación de unos pocos argumentos a una función a la vez y la devolución de otra función que se aplica a más argumentos. Aquí hay un ejemplo: <blockquote> // Función imparcial <br> función imparcial (x, y, z) { <br> devuelve x + y + z; <br> } <br> var partialFn = imparcial.bind (esto, 1, 2); <br> parcialFn (10); // Devoluciones 13 </blockquote></section>

## Instructions
<section id="instructions"> Rellene el cuerpo de la función de <code>add</code> para que use el curry para agregar los parámetros <code>x</code> , <code>y</code> y <code>z</code> . </section>

## Tests
<section id='tests'>

```yml
tests:
  - text: <code>add(10)(20)(30)</code> debe devolver <code>60</code> .
    testString: 'assert(add(10)(20)(30) === 60, "<code>add(10)(20)(30)</code> should return <code>60</code>.");'
  - text: <code>add(1)(2)(3)</code> debe devolver <code>6</code> .
    testString: 'assert(add(1)(2)(3) === 6, "<code>add(1)(2)(3)</code> should return <code>6</code>.");'
  - text: <code>add(11)(22)(33)</code> debe devolver <code>66</code> .
    testString: 'assert(add(11)(22)(33) === 66, "<code>add(11)(22)(33)</code> should return <code>66</code>.");'
  - text: Su código debe incluir una declaración final que devuelva <code>x + y + z</code> .
    testString: 'assert(code.match(/[xyz]\s*?\+\s*?[xyz]\s*?\+\s*?[xyz]/g), "Your code should include a final statement that returns <code>x + y + z</code>.");'

```

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js
function add(x) {
  // Add your code below this line


  // Add your code above this line
}
add(10)(20)(30);

```

</div>



</section>

## Solution
<section id='solution'>

```js
// solution required
```
</section>
