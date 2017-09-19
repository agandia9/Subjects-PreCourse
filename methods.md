<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">

## Methods

http://www.w3schools.com/js/functions.asp

*Simple JS Methods for example.*

```javascript
var today, someday, text;
today = new Date();
someday = new Date();
someday.setFullYear(2100, 0, 14);

if (someday > today) {
    text = "Today is before January 14, 2100.";
} else {
    text = "Today is after January 14, 2100.";
}
console.log(text)

```
👆🏼 Estos ejercicios se deberán hacer exclusivamente usando **METODOS**

---


### Strings
a) Puedes contar cuantas letras tiene tu nombre? 
```javascript
console.log(myName) // My Name has 4 letters 
```
**Check this:** http://bfy.tw/AlDi 👈🏼

b) Añade tu apellido e indica en que posición se encuentra
```javascript
console.log(myString)// Your first last name starts on position 5
```
 
c) Ahora, con tu apellido y nombre en la misma variable, muestra solo el nombre.
```javascript
console.log(myString) // My Name is Tony 
```
 
d) Ahora, solo tu apellido.
```javascript
console.log(myString) // My lastname is Stark
```

d1) Iguala el resultado a una variable nueva e imprímela por pantalla.
```javascript
console.log(myFirstString +", " + myNewString) // Tony Stark, Stark
```

e) Ahora, reemplaza tu nombre por "Mr/Ms" y vuelve a mostrar la variable con los cambios. 
```javascript
console.log(myNewString) // Hello, Mr. Stark 
```
 
f) Selecciona tu apellido y transfórmalo a MAYÚSCULAS.
```javascript
console.log(mySelection) // my lastname is STARK
```

g) Ahora declara una variable nueva e igualala a la anterior variable sumándole, además, un mensaje.
```javascript
var something = myFirstString + "is awesome"
console.log(something) \\ "Tony is awesome"

```

h) Ahora, puedes seleccionar la inicial de tu nombre y apellido y mostrarlas por pantalla?
```javascript
console.log(myFirstLastnameLetters) // S.Y
```

---

### Arrays
a) Declara tu nombre completo en una array y muéstralo por pantalla separando cada letra por "/"
```javascript
console.log(myName) // T/O/N/Y/S/T/A/R/K
```

b) Ahora solo selecciona tu apellido y muestra cada letra separada por "|"
```javascript
console.log(myName) // S|T|A|R|K
```

c) Ahora muestra cada letra de tu **nombre** con su posición (necesitarás un bucle **for**)
```javascript
console.log(myName) // 1º T, 2º O, 3º N, 4º Y
```
Resource: https://www.w3schools.com/jsref/jsref_split.asp

d)Como en el ejercicio anterior, pero seleccionando tu apellido
```javascript
console.log(myLastName) // 5º S, 6º T, 7º A, 8º R, 9º K
```
Resource: https://www.w3schools.com/jsref/jsref_length_array.asp

e) Puedes indicarme las iniciales de tu nombre y apellido? Como en el **ejercicio h** de la sección de strings
```javascript
console.log(myInitials) // T.S
```

f) Ahora, reformula la array, introduciendo tu nombre en primera posición, tu apellido en segunda, y además añade en otra posicion tu edad.
Muestra por pantalla solo tu nombre y tu edad en un solo mensaje.
```javascript
console.log(mySelector) // My name is TONY and i'm 40 years old
```

g) Prepara una función para añadir tu City a la array, muestra un mensaje mostrando el contenido de toda la array, así aseguraremos los cambios.
```javascript
console.log(myCityAdd) // City added to array! => Tony, Stark, 40, New York
```

h) Crea ahora, una funcion para eliminar la variable City y asegura los cambios.
```javascript
myCityAdd() // City added to array! => Tony, Stark, 40, New York
myCityDelete() // City deleted! => Tony, Stark, 40
```

j) Ahora, elimina el nombre y asegura los cambios
Resources: https://www.w3schools.com/jsref/jsref_shift.asp

k) Quiero volver a introducir mi nombre pero si lo introduzco utilizando push() estará en la última posición, como podria hacer para introducirlo en la primera posición?
Resources: https://www.w3schools.com/jsref/jsref_splice.asp

l) Ahora, declara una array con los números del 0 a 10 y muestra cada número multiplicado por dos.
```javascript
numbers = [...]
var multByTwo = numbers.map(...)
```

l1) Reformula la función para que puedas especificar por cual número debería multiplicar cada elemento de la array.

```javascript
var num = 3; // cada número se multiplicará por 3
function multByNum(num){
    var arrayMult = numbers.map(...)
    return arrayMult
}
```

Resource: https://www.w3schools.com/jsref/jsref_map.asp

m) Podrías mostrarlos en el orden inverso?
Resources: https://www.w3schools.com/jsref/jsref_sort.asp

n) Puedes indicarme que letras se repiten de tu nombre y cuantas veces?
```javascript
console.log(repeatLetters) // Tony Stark, the letter 'T' => 2 times.
```

n1) Ahora muestra por consola que letras NO se repiten y muestra tu nombre sin esas letras

```javascript
console.log(repeatLetters) // Tony Stark, the letters => o, n, y, s, a, r, k are not repeated, the name is => Ony Sark
```

---

### Numbers
a) Que hora es? Declara la hora como número y devuelvela como String 
```javascript
console.log(myString + myNumberStringify) // I'ts 10.45 of morning
```
*Hint* => https://www.w3schools.com/jsref/jsref_tostring_number.asp

b) Nono, que hora exactamente? Dime la hora sin minutos 
```javascript
console.log(myString) // It's around 10 of morning
```

c) Ahora, declara tu hora y muéstrala redondeada.
```javascript
console.log(...(10.34)) // 11!
```
*Hint* => https://www.w3schools.com/jsref/jsref_round.asp

d) Hagamos una calculadora. Primero, la suma.  
We can do a calculator, so let's do it! first, do a sum with two numbers
```javascript
console.log(sum) //The sum of 7+3 is 10
```

d1) Añade la resta...
```javascript
console.log(sum + rest) // The sum and rest of 7 and 3 is 10 and 4 
```

d2) Y la multiplicación
```javascript
console.log(sum + rest + mult) // 10, 4 and 21
```

d3) Por ultimo, la división
```javascript
console.log(sum + rest + mult + div) // 10, 4, 21 and 2.3
```

d4) Ahora, intenta multiplicar un número por una string, que devuelve?
```javascript
console.log(10*"hour") // ....?!
```

e) Podemos controlar este error con un condicional **if**?
```javascript
console.log(10*"hour") // You can't do this operation!
```


