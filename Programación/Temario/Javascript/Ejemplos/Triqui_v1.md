```js
   
// creamos el tablero
const tablero = [
//  c1  c2 c3
	[0, 0, 0],     // esta es la fila 0
	[0, 0, 0],     // esta es la fila 1
	[0, 0, 0],     // esta es la fila 2
];


// creamos una variable que maneja el turno
// si es el jugador a se pone en menos 1
// si es el jugador b se pone en uno
let turno = 1;


// creamos una variable para poner los textos del tablero
let vista_tablero = '    1   2   3\n   -----------\n';
for(let i=0; i<3; i++) {
	// extraemos los valores de las casillas del tablero
    let a = ' ';
    if (tablero[i][0] !== 0) {
        a = 'X';
    }
    let b = ' ';
    if (tablero[i][1] !== 0) {
        b = 'X';
    }
    let c = ' ';
    if (tablero[i][2] !== 0) {
        c = 'X';
    }
    // ponemos la info dentro de la variable del tablero
    vista_tablero += `${i + 1} | ${a} | ${b} | ${c} |\n`
}
// agregamos la linea final del tablero
vista_tablero += '   -----------\n';
// escribimos el contenido del tablero
console.log(vista_tablero);


// creamos una variable que habilita o deshabilita la ejecución
let ejecutar = true;

// mientras ejecutar sea verdadeto
while(ejecutar) {
	// creamos una variable que indica si debemos pedir datos de usuario
    let pedir_datos = true;
    while (pedir_datos) {
        let fila_u = -1;
        let pedir_fila = true;
        while (pedir_fila) {
	        const c_file = prompt('Ingrese una fila:');
            fila_u = (
	            parseInt(c_fila) + 1
            );
            if (fila_u >= 0 && fila_u < 3) {
                pedir_fila = false;
            } else {
                alert('fila invalida')
            }
        }
        let columna_u = -1;
        let pedir_columna = true;
        while (pedir_columna) {
	        const c_columna = prompt('Ingrese una columna:');
            columna_u = (
	            parseInt(c_columna) + 1;
            );
            if (columna_u >= 0 && columna_u < 3) {
                pedir_columna = false;
            } else {
                alert('columna invalida')
            }
        }
        tablero[fila_u][columna_u] = turno;
        turno = turno * -1;
        pedir_datos = false;
    }
    
	let vista_tablero = '    0   1   2\n   -----------\n';
    for(let i=0; i<3; i++) {
        let a = ' ';
        if (tablero[i][0] !== 0) {
            a = 'X';
        }
        let b = ' ';
        if (tablero[i][1] !== 0) {
            b = 'X';
        }
        let c = ' ';
        if (tablero[i][2] !== 0) {
            c = 'X';
        }
        vista_tablero += `${i + 1} | ${a} | ${b} | ${c} |\n`
    }
    vista_tablero += '   -----------\n';
    console.log(vista_tablero);


	ejecutar = false;
}

```

