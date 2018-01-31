# Identifica
El ejercicio sconsiste en leer el codigo javascript e identificar las funciones globales, locales, funciones de callback, expresions, statement, clousure, scope, contextos de ejecucion, que funciones forman parte de la pila de ejecucion (stack execution) y que funciones forman parte de la cola de eventos (event queue).
## Funciones globales
Son las funciones que están definidas en el ámbito global.
```js
$(document).ready(function() {
    ...
}
```
## Funciones locales
Son las funciones que se declararon dentro de otra función.
```js
    console.log(...);   
    function activeButton() {...}
    function desactiveButton() {...}
    function longitud(input) {...}
    function soloNumeros(input) {...}
    function isValidCreditCard(numberCard) {...}
```
## Funciones de callback
Son funciones que sirven de parámetro de otra función.
```js
var creditCardNumber = soloNumeros(longitud(numberCard));   //La función longitud se convierte en parámetro de soloNumeros
```
## Expresions
Son funciones declaradas en una expresión.
```js
var creditCardNumber = soloNumeros(longitud(numberCard));  //La variable creditCardNumber toma el valor de las funciones

```
## Statement
Son funciones declaradas para su posterior llamado.
```js
soloNumeros(), longitud () //llamados en línea 45
activeButton() //línea 65
desactiveButton() // línea 68 y72
```
## Clousure
Son funciones que acceden a las variables que fueron creadas en la función
```js
soloNumeros(longitud(numberCard));  //soloNumeros accede a las variables usadas en longitud (input).
```
## Scope

## Contexto de ejecución

## Stack execution

## Event queue
