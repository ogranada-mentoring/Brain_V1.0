Javascript ofrece varias herramientas para gestionar el control de flujo de la aplicación.

## If - Else
El `if` o `si logico` es una instrucción que ejecuta una sentencia (vea [[Expresiones y Sentencias]]) si y solo si una expresión es evaluada como verdadera. Si la condición es evaluada como falsa (`else`), otra sentencia puede ser ejecutada.

Ejemplos:

```js
/*
if ( <expresion> ) <sentencia> else <otra sentencia>
*/
const edad = 10;
if (edad > 18) console.log('Puede votar!') else console.log('No puede votar.')



const michu = {
	name: 'michu',
	breed: 'felino',
};
// Separamos todo en varias lineas, se lee mejor
if (michu.breed === 'felino')
	console.log('Es un lindo gatito!');
else
	console.log('No la mamá...');


const baby = {
	name: 'Baby Sinclair',
	breed: 'dino',
};
// Separamos todo en varias lineas, se lee mejor
if (baby.breed === 'dino') {
	console.log('No la mamá...');
} else {
	console.log('Es un lindo gatito!');
}

```


## Switch

La instrucción switch evalúa una expresión, comparando el valor de esa expresión con una serie de casos (`cases`) y ejecuta las sentencias asociadas a ese `case`, así como las declaraciones en los case que siguen hasta que encuentra una sentencia de ruptura (`break`). También es posible agregar un caso que se ejecuta cuando ningún otro caso ha sido valido (`default`).

Ejemplos:

```js
/*
switch ( <expresion> ) {
	case <valor>:
		<sentencia 1...>
		<sentencia 2...>
		<sentencia 3...>
		...
		<sentencia n...>
		break;
	case <valor>:
		<sentencia 1...>
		<sentencia 2...>
		<sentencia 3...>
		...
		<sentencia n...>
		break;
	default:
		<sentencia 1...>
		<sentencia 2...>
		<sentencia 3...>
		...
		<sentencia n...>
		break;
}
*/


const baby = {
	name: 'Baby Sinclair',
	breed: 'dino',
};

switch ( baby.breed ) {
	case 'felino':
		console.log('Es un lindo gatito!');
		break;
	case 'dino':
		console.log('No la mamá...');
		break;
	default:
		console.log('Nada por decir...');
		break;
}
```

