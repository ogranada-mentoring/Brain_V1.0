### Para la consola de desarrollo:

En javascript podemos escribir datos de las siguientes maneras:
```js
// console.log( COSA QUE QUEREMOS ESCRIBIR )
console.log( "Hola Mundo!" )
console.log( 'Este es otro saludo' )
console.log( `Este es un ejemplo de comilla francesa ${1111}` )
```

### Para el navegador:

En javascript podemos escribir datos de las siguientes maneras:
```js
// console.log( <COSA QUE QUEREMOS ESCRIBIR> )
alert( "Hola Mundo!" )
alert( 'Este es otro saludo' )
alert( `Este es un ejemplo de comilla francesa ${1111}` )
```

Además podemos solicitar datos de teclado de la siguiente manera:
```js
// prompt( <El mensaje que quiere mostrarle al usuario> )
prompt('Ingrese el tamaño del tablero')
```
El resultado de `prompt` siempre va a ser una cadena, se recomiendan las funciones `parseInt` y `parseFloat` para convertir las cadenas en números.
