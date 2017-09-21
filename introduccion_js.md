<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">

## VARS, LOOPS, CONDITIONALS

#### Variable:

Una variable es un contenedor que sirve para almacenar datos.
En javascript utilizamos la palabra reservada ``` var ``` para declarar una variable. 

Ejemplos:

Creamos una variable que nos almacena un número:
```javascript
var skylab = 10
```

Creamos una variable que nos almacena un cadena de texto:
```javascript
var skylab = 'coders'
```

Creamos una variable que nos almacena un array:
```javascript
var skylab = ['coders', 'academy', 7]
```

Creamos una variable que nos almacena un objeto:
```javascript
var skylab = { lenguaje: 'javascript', stack: 'MEAN', angular: 4 }
```

#### Loops:

<img src="http://3.bp.blogspot.com/-f6yRbQQ_lCU/VXaV3w5WEbI/AAAAAAAAAJI/0-czJApvhEc/s1600/C-For-Loop-Statement.jpg" style="width:25%;height:25%;">


Un loop nos sirve para iterar tantas veces como queramos y aplicar la misma lógica cada vez.

En javascript hay 3 tipos de loops básicos:

**for**  
El bucle for lo utilizaremos cuando tengamos que repetir alguna lógica un numero **determinado** de veces.
```javascript
for(var i=0;i<10;i++){
    //code here
}
```

**while**   
El bucle while lo utilizaremos cuando tengamos que repetir alguna lógica un numero **indeterminado** de veces y queremos que se ejecute mientras se cumpla una condición específica, esta condición se comprobará al **inicio** de cada iteración.

```javascript
while(condition){
    //code here
}
```

**do while**  
El bucle while lo utilizaremos cuando tengamos que repetir alguna lógica un numero **indeterminado** de veces y queremos que se ejecute mientras se cumpla una condición específica, esta condición se comprobará al **final** de cada iteración.
```javascript
do{
    //code here
}while(condition)
    
```


#### Conditionals
<img src="http://cess.nyu.edu/wp-content/uploads/2012/01/ifcond.jpg" >


Los condicionales **if**, **else if** y **else** nos sirven para ejecutar un trozo de código dependiendo de si cumple una determinada posición o no.

```javascript
var a = 10
var b = 7

if (a<b) {
 //code here
} else {
 //code here
}
```


```javascript
var a = 10
var b = 7
var c = 3

if (a<b) {
 //code here
} else if (c<b){
 //code here
} else {
 //code here
}
```

---

**Exercises:** // faltan 5

a) Declara tu nombre y muéstralo por consola: 

```javascript
console.log(name) //Mark
```

b) Declara tu edad y muéstralo por consola:

```javascript
console.log(age) //38
```

c) Declara tu nombre, tu apellido y tu edad en un array en diferentes posiciones y muéstrala por consola:

```javascript
console.log(info) //['Mark', 'Zuckerberg', 21]
```

d) Declara tu nombre y tu edad dentro de un objeto y muéstralo por consola:

```javascript
console.log(data) //{ name: 'Mark', age: 21}
```

e) Ahora utiliza el array que has creado anteriormente para recorrerlo y mostrar una a una todas las posiciones del array.

```javascript
 //'Mark'
 //'Zuckerberg'
 //21
```

f) Crea una estructura condicional que imprima el número mayor entre dos números.

```javascript
var a = 25
var b = 12
if( a < b) ...

//25
```

f1) Crea otra condicion else if para contemplar la posibilidad de que los dos números sean iguales:
```javascript
var a = 25
var b = 12
else if(...)
// The numbers are equal
```

g) Crea una array de 5 numeros, y recorrela, mostrando además un mensaje cuando, esté a la mitad, muestre un mensaje 'We are in the middle of loop'.
```javascript
for(...){
    if(...){"We are in the middle of loop"}
}
```

g1) Declara tu nombre y tu edad dos variables y crea un condicional para, en caso de no coincidir con tus datos, mostrar un error
_Hint_: https://www.w3schools.com/js/js_comparisons.asp **(Logical Operators section)**

```javascript
var myName...
var myAge...
if(oneThing && otherThing...){"this is not you!"}
else{"Hi!! Glad to see u again!"}
```

g2) Crea una array, introduce los datos anteriores y unos cuantos más de forma que al recorrer la array, muestre un mensaje cuando encuentre tus datos.

```javascript
for(...){
    if(...){"We find your data!" + data[...]}
}
```

