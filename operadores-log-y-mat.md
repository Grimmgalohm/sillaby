# Operadores Lógicos y Matemáticos.

## Operadores matemáticos.

Muy seguramente, desde la educación primaria, has estado muy relacionado con los operadores matemáticos y su función en la aritmetica y las matemáticas en general.
* Suma (+)
* Resta (-)
* Multiplicación (*)
* División (/)

Para operaciones como las potencias, raices, seno, etc, tenemos funciones específicas, que, por el momento, no ahondaremos.
<br>

Está de más explicar el uso de cada uno de los operadores, sin embargo, trabajaremos con cada uno para ver lo que se puede llegar a hacer.

```
//Declara una variable con el nombre correspondiente a la operación que vas a realizar.

let suma = 5+5; //dentro debe ir la operación que vas a realizar y entre numeros el signo.

//Imprime en la terminal la variable con la funcion console.log

> console.log(suma);

//Verifica que el resultado que te aparezca sea el correcto, es decir:

> 10
```

Otra forma de operar, en caso de que los valores se encuentren dentro de variables diferentes, es asignandolos a una nueva variable, ejemplo:

```
//Con el mismo ejemplo de la suma declara dos variables.

let numero1 = 5;
let numero2 = 5;

let resultado = numero1 + numero2;

//Ahora, imprime la variable resultado en la terminal.

> console.log(resultado);

```
También se puede imprimir el resultado de la operación directamente a consola con la función console.log.

```
//Escribe en tu documento

> console.log(5+5);

//Ahora compila el documento para que te mueste el resultado en la terminal

> node main.js

```
### Los operadores restantes.
```
const a = 10;
const b = 5;
let res;

// + Para sumar dos o más números.
 res = a + b; 
console.log(res); //Si imprimes la variable res, el total de la suma debe ser 15.

// - Para restar.
res = a - b; 
console.log(res) //Al imprimir la variable res, el total de la resta debe ser 5.

// *(asterisco) para multiplicar.
res = a * b;
console.log(res); //Al imprimir la variable res, el total de la multiplicación debe ser 50.

// /(diagonal) para dividir.
res = a / b;
console.log(res); //Al imprimir la variable res, el total de la división debe ser 2;

// ** Doble asterisco para elevar un número a cierta potencia.
res = a ** b; // Al imprimir la variable res, el total de elevar "a" a la potencia "b" debe ser 100,000.
console.log(res);

// %(signo de porcentaje) que nos dá como resultado el resíduo de la división entre dos números.
res = a % b;
console.log(res); //Al imprimir la variable res, el residuo de la operación debe ser 0.
```
Con estos operadores aritméticos se pueden construir operaciones más complejas haciendo uso de los paréntesis "()" y las corcheas "[]".
```
let total = 2*[2+(2+2)];
console.log(total); //El resultado al imprimir la variable total, debe ser 12.
```
## Operadores Lógicos (Booleanos)

Estas expresiones son útiles al momento de evaluar y discriminar datos, dando como resultado true o false, es decir, verdadero o falso. Esto nos permite usarlos para determinar si se continúa por uno u otro "camino" o si un ciclo se termina o continúa. Se dividen en dos grupos: operadores lógicos y operadores relacionales.

### Operadores Lógicos.

#### AND (&&).
Sólo regresa true si todos los datos tienen un valor verdadero(true), si no, da como resultado false. Tabla de verdad:

```
x       y       (x&&y)
true    true    true

true    false   false

false   true    false

false   false   false
```

Cualquier dato que no sea igual a los otros hará que el resultado sea false(o todos coludos o todos rabones).

#### OR (||)
Regresa el resultado true, si uno solo de los operandos es verdadero(true). Tabla de verdad:

```
x       y       (x||y)
true    true    true

true    false   true

false   true    true

false   false   false
```
Si ningún operando es igual a true, da como resultado false.

#### NOT(!)
Invierte el valor del operando, es decir, si el operando es true, lo convierte en false. Ejemplo:
``` 
x       !x
true    false

false   true
``` 
#### Operadores Relacionales.

Nos ayudan a evaluar cantidades (números), ver qué operando es mayor, menor, igual o diferente. Ejemplo:
```
// "Menor que", evalúa si "x" es MENOR a "y".
console.log(x < y)

// "Menor o igual que", evalúa si "x" es MENOR O IGUAL a "y".
console.log(x <= y)

// "Mayor que", evalúa si "x" es MAYOR que "y".
console.log(x > y)

//"Mayor o igual que", evalúa si "x" es MAYOR O IGUAL que "y".
console.log(x >= y)
También podemos usar variables para evaluar igualdades o desigualdades entre cantidades u operandos.

//"Igual o similar a", evalúa si el operando es igual en valor, sin tomar en cuenta el tipo de dato.
( x == y)

//"Exactamente igual a", evalúa si el operando es estrictamente igual en valor y tipo de dato.
(x === y)

//"Desigualdad", evalúa si entre los operandos hay alguna desigualdad, es decir, que no sean iguales o similares.
(x !== y)
```
**Consejo** Ten en cuenta que el signo "=" (igual matemático) es el que utilizamos para asignar valores a las variables o constantes, por lo tanto, no nos sirve para operar como igualdad, es un error común usarlo en vez de "Igual a: ==". Procura siempre usar "estrictamente igual a(===)", de esa manera puedes evitar errores manejando tus datos.