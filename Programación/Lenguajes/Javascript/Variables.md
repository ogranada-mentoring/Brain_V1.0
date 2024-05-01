En Javascript las variables pueden ser declaradas mediante 3 maneras:

* Usando la palabra reservada `var`.
* Usando la palabra reservada `let`.
* Usando la palabra reservada `const`.

Estás palabras reservadas permiten crear variables, pero cada una tiene sus particularidades:

#### Var 

* Permite re-declarar variables.
* Permite reasignar los valores de una variable.
* Está limitada por contexto de función o módulo (su alcance es válido dentro de una función o del módulo en el que se creó).
* Es afectada por el [[Hoisting]].

Ejemplos:
```js
var a = 1;
var b = 'sample';
var b = false;
```

#### Let

* Permite reasignar los valores de una variable.
* **No** permite re-declarar una variable.
* Limita el alcance de la variable al bloque sintáctico que la contiene.
* No es afectada por el [[Hoisting]].

Ejemplos:
```js
let a = 1; // crea a con un 1 adentro
a = 2; // cambia el valor de a sin problema por 2
let b = 'sample';
let b = false; // lanza un error por que 'b' ya fue creado en este contexto
{ // inicio de sentencia de bloque
	let b = 10; // no causa error por que es un contexto distinto
}
```

#### Const

* No permite reasignar los valores de una variable, sin embargo permite alterar el contenido si la variable contiene el objeto.
* **No** permite re-declarar una variable.
* Limita el alcance de la variable al bloque sintáctico que la contiene.
* No es afectada por el [[Hoisting]].

Ejemplos:
```js
const a = 1;
a = 2; // lanza un error por que no puede cambiar una constante
const b = 'sample';
const b = false; // lanza un error por que 'b' ya fue creado en este contexto
{ // inicio de sentencia de bloque
	const b = 10; // no causa error por que es un contexto distinto
}

const obj = {}; // crea un objeto
obj.sample = 10; // cambia una propiedad del objeto obj, pero no cambia obj.
```
