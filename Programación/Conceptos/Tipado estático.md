El tipado estático hace referencia a la forma en que se le indica al compilador/intérprete de un lenguaje cuál es el tipo de dato (y por ende cuanta memoria requiere) de una variable.

En lenguajes como c++ se crean variables de la siguiente manera.

```cpp

int main(int argc, char *argv[]){
  int value = 0;
  char option = ‘y’;
  return 0;
}

```

en el código anterior vemos  las variables `argc`, `argv`, `value` y `option` tienen definidos de manera explícita los tipos `int`, `char*`, `int` y `char` respectivamente.