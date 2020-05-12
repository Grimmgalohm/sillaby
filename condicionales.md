# Condicionales

También llamadas estructuras dedecisión, le permiten al programa tomar uno u otro camino al ejecutarse, según los parámetros que hemos diseñado para que tome en cuenta. 
<br/>
Podemos ponerlo en un ejemplo de la vida cotidiana, en donde al momento de hacer el super, discriminamos entre productos para satisfacer nuetros gustos personales y hacer rendir el dinero que destinamos a la comida de la quincena. Así pues, al darle ciertos parámetros al programa, este se encarga de discernir entre qué hacer con la información que se le otorga.
<br/>
Como estructuras de decisión tenemos:
## if
Esta estructura es muy fácil de entender, se basa en la palabra "**SI**".
<br/>
"**SI**" hay en una lista de números del uno al diez un 5...
<br/>
"**SI**" se presiona la flecha hacia arriba...
<br/>
"**SI**" la fecha de caducidad del producto aún no llega...
<br/>
Etc, etc.
<br/>
Dentro de nuestras líneas de código, se utiliza así.
```
//Escribimos la palabra reservada:
if() 
//dentro de los paréntesis introducimos una expresión booleana, que el programa entenderá como el parámetro a tener en cuenta al momento de decidir.
if( x >= 10 ){
    
}
//Así, dentro de las llaves introduciremos el código que se ejecutará en caso de que se cumpla la condición.
if( x >= 10 ){
 console.log("Yep, this is!");
 }
```
**IF** viene acompañado de **Else** que nos permite introducir una segunda opción de un "qué a ejecutar" en caso de que la primera condición no se cumpla, es decir, es un "si no..."

```
//Usamos la palabra reservada else seguido de las llaves donde irá nuestro código alternativo.
//Con else no es necesario poner un parámetro, ya que el código se ejecuta SOLO cuando la primera condición no se cumple.
if( x >= 10 ){
 console.log("Yep, this is!");
 }else{
     console.log("Whut?!");
 }
```
## Switch

Es un condicional que permite una cantidad "discreta" de casos, que evitan depender de una expresión booleana, y se enfocan en situaciónes más especificas.
<br/>
Para ello debemos de entender la estructura de la condición **Switch**
```
//Tenemos una variable que vamos a evaluar con switch
let x = 5;
//Utilizamos la palabra reservada switch, seguida de dos paréntesis, dentro de los cuáles tendremos nuestra variable a evaluar.
switch (x){
}
//Dentro de las llaves tendremos los casos con las acciónes a llevar a cabo por el programa, se utiliza la palabra reservada **case** seguido de, a qué se tiene que parecer, para ejecutar la instrucción.
switch(x){
    
    case 1: //*
    console.log("Nope") //**
    break; //***
}
//*En este caso x debe ser estrictamente igual a 1 (un entero);
//**Esta es la instrucción que se debería ejecutar si el caso se cumple.
//***Se utiliza break; al final de cada caso para evitar que se ejecuten todos los casos (si no es lo que se quiere).
```
Cabe mencionar que Switch utiliza la comparación estricta, lo que quiere decir que si el argumento es 7.5 y ningúno es exactamente 7.5 la condición no se cumple y no se ejecuta más que el caso por defecto (default), si es que existe, si no, el programa continúa con lo que esté escrito fuera del Switch.

```
//Switch puede ser usado para comparar texto, tal como una palabra.
//En estos casos, recuerda que el texto va siempre dentro de comillas dobles ""
let x;
switch(x){
    case "Gus":
    console.log("Hola!")
    break;
    case "Wens":
    console.log("Bienvenido!")
    break;
    default:
    console.log("No name :(")
}
```