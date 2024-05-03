Los ciclos son instrucciones que permiten ejecutar una sentencia multiples veces.

Javascript tiene 3 ciclos básicos:

## While (mientras)
El ciclo while ejecuta algo `mientras` una condición sea verdadera:

Ejemplos:

```js

// while ( <expresion> ) <sentencia> 

const edad = 1;
while (edad > 18) { // sentencia tipo bloque
	console.log('tiene ' + edad + ' años');
	edad = edad + 1;
} // fin de sentencia tipo bloque
```


## Do-While (haga mientras)
El ciclo do-while ejecuta algo `mientras` una condición sea verdadera, sin embargo, ejecuta la sentencia _antes_ de validar la expresión:

Ejemplos:

```js

// do  <sentencia>  while ( <expresion> )

const edad = 1;
do { // sentencia tipo bloque
	console.log('tiene ' + edad + ' años');
	edad = edad + 1;
} // fin de sentencia tipo bloque
while (edad > 18);
```

## For (para)
El ciclo para ejecuta algo hasta que se cumplan unas condiciones especificas, en éstas hay una expresión de iniciación, una expresión de comparación (que retorna verdadero o falso) y una expresión de cambio (usada comúnmente para incrementar un valor):

Ejemplos:

```js

// for (
//    <expr. de iniciación> ;
//    <expr. de comparación> ;
//    <expr. de incremento>
// ) <sentencia>

for (
	let contador = 0;
	contador < 10;
	contador = contador +1
) console.log(`EL contador es ${contador}`)



