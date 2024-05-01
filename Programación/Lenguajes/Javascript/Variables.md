En Javascript las variables pueden ser declaradas mediante 3 maneras:

* Usando la palabra reservada `var`.
* Usando la palabra reservada `let`.
* Usando la palabra reservada `const`.

Estás palabras reservadas permiten crear variables, pero cada una tiene sus particularidades:

#### Var 

* Permite redeclarar variables.
* Permite reasignar los valores de una variable.
* Está limitada por contexto de función o módulo (su alcance es válido dentro de una función o del módulo en el que se creó).
* Es afectada por el [[Hoisting]].

#### Let

* Permite reasignar los valores de una variable.
* **No** permite redeclarar una variable.
* Limita el alcance de la variable al bloque sintáctico que la contiene.
* No es afectada por el [[Hoisting]].


#### Const

* No permite reasignar los valores de una variable, sin embargo permite alterar el contenido si la variable contiene el objeto.
* **No** permite redeclarar una variable.
* Limita el alcance de la variable al bloque sintáctico que la contiene.
* No es afectada por el [[Hoisting]].
