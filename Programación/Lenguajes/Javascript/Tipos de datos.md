En javascript tenemos los siguientes tipos de datos:

## Number
Sirve para representar cantidades numéricas. estas cantidades pueden ser positivas, negativas, reales, exponenciales, infinitas.

Ejemplos:
```js
0
10
-11
1.4
10e3
Infinite
-Infinite
```

## String
Sirve para representar un grupo de caracteres (texto). Las cadenas se caracterizan por estar rodeadas por comillas (ya sean sencillas `'`,  dobles `"` o francesas `` ` ``). Las comillas francesas (o back ticks) también sirven para hacer string interpolation.

Ejemplos:
```js
'Hola, soy una cadena de caracteres'
"Hola"
let nombre = 'Juan';
console.log(`Hola, soy ${nombre}`); // Hola, soy Juan 
```

## Boolean
Sirve para representar valores de verdad (verdadero o falso).

Ejemplos:
```js
true;
false;
let a = true;
let b = false;
```

## Null

Es una valor que representa una dirección de memoria que está separada y que contiene un valor que hace referencia al vacío.

Ejemplos:
```js
null;
let a = null;
```

## Undefined

Es una valor que representa una dirección de memoria que separada y se limpió pero no tiene nada especifico asignado. Cuando se crean variables sin asignar valores éstas tienen por valor `undefined` automaticamente.

Ejemplos:
```js
undefined;
let a; // contiene undefined
let b = undefined;
```

## Object

Un objeto es una unidad de datos que puede contener atributos de cualquier tipo de datos. Los objetos sirven para describir cualquier estructura de datos compleja. Los objetos se crean con los caracteres llave (`{}`) (No confundir con sentencias de bloque) o con la función auxiliar de creación de objetos.

Ejemplos:
```js
let objeto_vacio = {};
let objeto_con_atributo = {
	a: 1 // contiene un atributo llamado a que contiene un 1
};
let objeto_3 = Object.create({})
```

Teniendo en cuenta lo anterior, podemos decir que existen estructuras de datos más complejas, como los Arrays.
## Array

Teniendo en cuenta lo anterior, los Arrays (o arreglos) son Objetos, pero éstas estructuras tiene propiedades especiales (por ejemplo, `length`). Los arreglos son muy usados por que permiten almacenar una colección de datos y acceder a ellos de manera grupal o individual.

Los Arrays tienen algunas ayudas  especificas del lenguaje, como el uso de los corchetes (`[]`) que permiten crear arreglos fácilmente:
```js
let arreglo = [];
```
Los corchetes también sirven manipular su contenido:
```js
arreglo[0] = 1;
console.log(arreglo[0]);
```

Los arreglos pueden almacenar datos de cualquier tipo, además, cada `casilla` tiene un número para identificarla, la primera usa el número 0, la segunda el 1, la tercera el 2 y así sucesivamente.

Ejemplos:
```js
let arreglo = [];
let arreglo_con_datos = [1, 2, 'a']
let tablero = [
	[1, 2, 3],
	[4, 5, 6],
	[7, 8, 9],
];
console.log(tablero[0][1]) // escribe 2
console.log(tablero[1][1]) // escribe 5
console.log(tablero[2][2]) // escribe 9
```

## Symbol

Es un elemento que es único, es decir, no repetible. En muchos casos se usa para crear elementos especiales que son usados por javascript para ejecutar cosas especiales del lenguaje.

Ejemplos:
```js
const sym1 = Symbol();
const sym2 = Symbol("foo");
const sym3 = Symbol("foo");
// sym2 es diferente de sym3
```

## BigInt

Es un tipo de dato que representa cantidades numéricas, pero a diferencia del tipo `Number` fue creado para soportar números muy grandes. Pueden ser creadors poniendo el numero con una `n` al final o usando la función `BigInt`.


Ejemplos:
```js
const previouslyMaxSafeInteger = 9007199254740991n;
const alsoHuge = BigInt(9007199254740991);
```


# Operador typeof

EL operador `typeof` permite saber cual es el tipo de dato de un elemento.

Ejemplos:
```js
typeof 9007199254740991n // bigint
typeof 'a' // string
persona = { edad: 24 };
typeof persona // object
```
