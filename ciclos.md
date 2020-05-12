# Ciclos

Como su nombre lo indican, son fragmentos de código que se repiten. También conocidos como búcles o loops, en inglés, nos sirven para realizar acciónes que pueden ser repetitivas y ahorrarnos tiempo y código.
<br/>
Contamos con:

* While
* Do, while...
* For.

## While
Tenemos dos ejemplos de este búcle, por un lado está **while(true)** que es básicamente un búcle infinito, que va a repetir el código que se encuentra dentro de las llaves hasta que nosotros terminemos el programa.
```
while(true){
    console.log("Repeat");
    
}
```
Por otro lado está **While(boolean-expression)** que nos permite ejecutar el código en un búcle, que continúa hasta que se deja de cumplir la condición.
<br/>
```
while( a <= 10 ){
    console.log("Ja");
}
```

## Do, While...
Esta estructura de repetición nos garantiza que, lo que esté dentro de las llaves se va a ejecutar al menos una vez, que con el caso de while, si la condición no se cumple, el código puede ni siquiera ejecutarse.
```
do{
    console.log("This is some example");
}while( a <= 10 );
```

## For
Se utiliza para búcles que necesiten repetir el cuerpo (dentro de las llaves) un número determinado de veces.
<br/>
La estructura de un "for loop" es la siguiente:
* La variable de inicio de cuenta, que puede ser i, j, etc. A esta variable (generalmene) se le asigna el número 0 (o desde donde la cuenta comience).
* La expresión que determina si se ha concluído o no la cuenta.
* Si en el paso anterior la cuenta no corresponde con la expresión, se aumenta en uno la variable i y se vuelve a ejecutar el código dentro de las llaves.
```
for(let i = 0; i < 10; i++){
    console.log("Esto tiene que estar escrito 10 veces");
}
```

## Casos de uso.
* **While:** Lo utilizamos cuando queremos repetir una instrucción un número indefinido de veces.
* **Do, while:** Se usa cuando quieres ejecutar una instrucción un número de veces indefinido, pero, que se ejecute una vez al menos.
* **For:** Se usa cuando quieres repetir una instrucción un número especifico de veces.