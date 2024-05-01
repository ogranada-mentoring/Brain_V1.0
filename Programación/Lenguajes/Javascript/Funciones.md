En javascript las funciones pueden ser de dos tipos.

### Función clásica:
Es una función que tiene un contexto propio, se crea usando la palabra reservada `function`, además puede recibir un conjunto de argumentos.

```javascript
function sayHi(name, age) {
	console.log(`Hello ${name}, you are ${age} years old.`)
}
```

### Función flecha
Es una función que recibe su nombre por que usa un igual y un mayor que a manera de flecha (`=>`). Ésta no tiene contexto propio, además, el cuerpo de esta puede ser una sentencia o una expresión.

```javascript
cont sayHi = (name, age) =>
	console.log(`Hello ${name}, you are ${age} years old.`);

```