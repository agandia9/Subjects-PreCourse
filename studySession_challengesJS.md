<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">
## Final Challenges (JS)!

a) Escribe una funcion en la que, declarando una array con los numeros del 1 al 9, muestres por pantalla los numeros unidos por parejas (1-2, 2-3, 3-4...), además, cada elemento de la  pareja deberá estar multiplicada por 2.
```javascript
function showNums(){
    var nums = [1,2,3,4,5,6,7,8,9]
    for(var i = 0; i < nums.length-1; i++){
        var pairs = []
        ...
    }
}
// output => 
//1ª pareja 2 - 4
//2ª pareja 4 - 6
//3ª pareja 6 - 8
//4ª pareja 8 - 10
//5ª pareja 10 - 12
//6ª pareja 12 - 14
//7ª pareja 14 - 16
//8ª pareja 16 - 18 
```
*Hint:* Métodos útiles => push() - join() - map()

a1) La funcion debería aceptar la array a tratar como argumento. 
```javascript
function showNums(1,2,3,4,5){
    var nums = arguments...
    nums.map(...)
}
// output => 
// 1ª pareja 2 - 4
// 2ª pareja 4 - 6
// 3ª pareja 6 - 8
//... 
```

a2) Pasa también el numero a multiplicar a la función como argumento
```javascript
function showNums(1,2,3,4,5,...,12){ //<= el último número de arguments lo podemos tratar como el numero multiplicador...
} 
// output => 
// El numero escogido es: 12
// 1ª pareja 12 - 24
// 2ª pareja 24 - 36
// 3ª pareja 36 - 48
// 4ª pareja 48 - 60
// 5ª pareja 60 - 72 
// ...
```

a3) La función debería ser capaz de recibir el numero de parejas que queremos devolver del total.
```javascript
function showNums(1,2,3,4,5,...,12, 3){ // <= ahora, el último numero lo podriamos tomar como el delimitador
} 
// output => 
// El numero escogido es: 12
// Se quieren mostrar las 3 primeras parejas
// 1ª pareja 12 - 24
// 2ª pareja 24 - 36
// 3ª pareja 36 - 48
```

---

b) Volvemos a la numeros...
Podrias hacer una funcion que mostrara por pantalla la serie *Fibonacci*?
https://www.mathsisfun.com/numbers/fibonacci-sequence.html

```javascript
function fibo(){}
// output: 0 1 1 2 3 5 8...
```

b2) Puedes añadir además, la posición de cada resultado?

b3) Ahora, inserta los resultados en una array y muestralos todos juntos de una manera amigable.

b4) Ahora, el usuario debería ser capaz de especificar la posición de la serie hasta donde queremos llegar.

```javascript
function fibo(10){}
//... 55 - pos 10º
```

b5) Ahora, muestra los resultados en forma piramidal:
```javascript
function fiboPymamid(num){}
0 
0 1 
0 1 1
0 1 1 2
0 1 1 2 3
0 1 1 2 3 5
0 1 1 2 3 5 8 //To position. num
0 1 1 2 3 5 
0 1 1 2 3
0 1 1 2
0 1 1
0 1 
0
```

---

c) **Simple Scripting program**. Crea un programa que transforme un número de 4 dígitos en otro diferente con las posiciones de los dígitos cambiadas, creandio un nuevo código
```javascript
var code = 3712;
function codeScript(code){}
//output:
 ⬇︎//First call to codeScript()
- 7123
 ⬇︎//Second call to codeScript()
- 1237
 ⬇︎//Third call to codeScript()
- 2371
// At Four call, should return the original value
```
**El primer numero se traslada a la última posicion. El segundo, el tercero y el cuarto suben una posición.**

c2) Ahora, el usuario debería poder introducir como parámetro dos códigos a la vez y devolver los dos códigos encriptados (Los dos códigos se deberían encriptar en la misma función)
```javascript
function codeScript(code1, code2){}
```

c3) Ahora, vamos a añadir un nivel más de seguridad. Despues de cambiar la posición de los dígitos, multiplicaremos a cada miembro por un numero cuya multiplicación no sea superior a 10. 
(Si es superior a 10, conseguiremos una multplicación de dos digitos y el código ya no sería de 4 valores)

c4) Ahora, implementa en otra funcion aparte el decrypter(), que recibirá como argumento un código encriptado (y correspondientemente multiplicado en el apartado c3) y nos devuelva el código desencriptado.

c5) Añade las dos funciones a la misma función padre, de forma que encripte y desencripte a la vez cuando termine de ejecutarse.
```javascript
function codeScript(code1, code2){... codeDecrypt(code1Encrypt,code2Encrypt)}
```

c6) El usuario podrá solo introducir letras, cada número del 0 al 9 corresponderá a varias letras. Podéis seguir este esquema.

```javascript
var dictionary = {
    0: ['A', 'K', 'T'],
    1: ['B', 'L', 'U'],
    2: ['C', 'M', 'V'],
    3: ['D', 'N', 'W'],
    4: ['E', 'Ñ', 'X'],
    5: ['F', 'O', 'Y'],
    6: ['G', 'P', 'Z'],
    7: ['H', 'Q', '.'],
    8: ['I', 'R', ','],
    9: ['J', 'S', ' ']
}
function codeScript("HI  ", "WE  ", "NEED", "HELP"){}
"HI..." = "dictionary[7][0]+dictionary[8][0]+dictionary[9][2]+dictionary[9][2]..."
```

---

d) Crea un programa que use la encriptacion Romana, como es?
Si tenemos la palabra SKYLAB, la palabra encriptada será SLKAYB.
Si divides la palabra original en 2 grupos obtienes:
- SKY
- |-|-|
- LAB 
Entonces, uniendo las primeras letras de cada grupo, las segundas y las terceras obtienes SLKAYB.

Entonces, el programa deberá recibir SKYLAB y retornar SLKAYB

d2) Programa el desencriptador, pasa como parámetro SLKAYB y que devuelva SKYLAB.

**Hint:** for decrypt, only catch the pair words like: **S** L **K** A **Y** B
 , then, you get SKY, the next step is catch the odd words, S **L** K **A** Y **B**, group the two groups and you get the original word.

d3) Agrupa la función **Encrypt** y **decrypt** en una unica función, de forma que introduzcas como parámetro SKYLAB y devuelva SKYLAB (con todas las transformaciones internas hechas y mostrando, entre medias, la transformación)

d4) Lo tienes? Prueba ahora con SKYLABCODERS. Cambia la función para que pueda aceptar palabras más largas.

---

e) Crea un programa al que le introduces un número como parámetro del 0 al 100 y devuelve el número transformado a alfabeto normal, es decir:
```javascript
sayItWithWords(5) => //output Five
sayItWithWords(23) => //output twenty-three
sayItWithWords(71) => //output seventy-one
```

_Hint_: 
```javascript
var units = ['', 'one', 'two', 'three', 'four', 'five', 'six', 'seven', 'eight', 'nine']
var tens = ['', '', 'twenty', 'thirty', 'forty', 'fifty', 'sixty', 'seventy', 'eighty', 'ninety']
var teens = ['ten', 'eleven', 'twelve', 'thirteen', 'fourteen', 'fifteen', 'sixteen', 'seventeen', 'eighteen', 'nineteen'];
```

e2) Ahora, el output debería ser capaz de, aparte de devolver el número traducido, devolver también los números por los que está formado:
```javascript
sayItWithWords(5) => //output Five, five / 5
sayItWithWords(23) => //output twenty-three, twenty + three / 20 + 3
sayItWithWords(71) => //output seventy-one, seventy + one / 70 + 1
```

e3) Cambia tu programa para que acepte cualquier número entre 0 y 1000.
```javascript
sayItWithWords(500) => //output five hundred , five hundred  / 500
sayItWithWords(233) => //output two hundred thirty three, two hundred + thirty + three/ 200 + 30 + 3
sayItWithWords(498) => //output four hundred ninety eight, four hundred + ninety + eight/ 400 + 90 + 8
```

---