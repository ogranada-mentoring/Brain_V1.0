Se le conoce como hoisting al proceso mediante el cual Javascript  ***mueve*** un elemento declarado (función o variable) al tope del contexto actual (función o módulo).

Esto ocurre por que la asignación de memoria de las variables que usan _var_ (véase [[Variables]]) y funciones en tiempo de compilación se hace al inicio de la sección de código, sin embargo, el uso y la inicializacion de variables siguen en los mismos lugares que se codificaron.

#### Ejemplo

```javascript

function demo() {
  console.log(hoisted);
  execution();
  function execution() {
    console.log(‘hello!’);
  }
  var hoisted = ‘I am hoisted’;
}

demo();

```

El ejemplo del código anterior tiene el siguiente resultado:

```bash
undefined
hello!
```

Cómo se ve en el resultado, pese a no lanzar un error por que la variable no se ha declarado, el valor que está almacenado es undefined. También vemos que aunque la función no se ha declarado aún aparentemente es posible invocarla.