En la mayoría de lenguajes de programación encontramos expresiones y sentencias.

## Expresión
En programación, una expresión es una combinación de constantes, variables o funciones, que es interpretada de acuerdo a las normas particulares de precedencia y asociación para un lenguaje de programación en particular. Ésta combinación genera un valor evaluado, es decir, la expresión es una representación de ese valor.

Ejemplos:
```js
2 + 2            // expresión aritmetica
2 < 3            // expresión relacional
isOk('yes')      // expresión con predicados
"Hola".length    // ...
```

además de eso, en varios lenguajes las expresiones pueden estar rodeadas por paréntesis, pues los paréntesis funcionan como elementos de agrupación de datos.

Ejemplos:
```js
(2 + 2)          // 4
((2 < 3))        // false
(((((3 + 3)) + ((2 + 2))))) // 10
```

## Sentencias

Son las unidades ejecutables más pequeñas de un programa, puede ser una línea de código escrita la cual tiene un final bien definido, para muchos lenguajes es un carácter (e.g. `;`  en C, C++, C#, Java y Javascript).

Hay un tipo de sentencias especiales que permiten agrupar varias sentencias adentro de ella misma, esta es la sentencia de bloque.

Ejemplos:
```js
2 + 2;           // sentencia que contiene una expresión aritmetica
2 < 3;           // sentencia que contiene una expresión relacional
isOk('yes');     // sentencia que contiene una expresión con predicados

{               // Inicio de una sentencia de tipo bloque
  doSomething(); // Una sentencia dentro de una sentencia de bloque
  y = y + 1;     // Otra sentencia dentro de una sentencia de bloque
}               // Fin de una sentencia de tipo bloque
```
