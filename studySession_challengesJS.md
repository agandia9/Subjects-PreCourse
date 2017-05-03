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
function showNums(1,2,3,4,5,...,12){ //<= el último número de arguments lo podemos tratar como el multiplicador...
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

c) **Simple Scripting program**. Create a program that transform a 4 number values code to diferents positions, making a new code.
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
**The first number, go to the last position. Second, third and four goes up.**

c2) Now, the user can introduce two different codes and should return the codes changed.
```javascript
function codeScript(code1, code2){}
```

c3) Now, we try to add a additional level of security. After change the position of numbers, we can multiplicy the values by 2.
*(we have a problem if the mult of numbers is > 10, choose numbers < 4 for make the code)*.
For asure the implementation of extra security level, do the properly console.logs().

c4) Now, do the DECRYPT function, call it before ends the codeScript function for asure the functionallity.
```javascript
function codeScript(code1, code2){... codeDecrypt(code1,code2)}
```

---

d) Create a program that use the Roman form for encrypt messages, how is that? Simple. If you have SKYLAB, the encrypted form is  SLKAYB...
If you divided the word in two groups of 3 letters, you get:
- SKY
- |-|-|
- LAB 
Then, join the S with L, K with A and Y with B, and you get SLKAYB.

So, make a program that, receive the message SKYLAB and returns the SLKAYB.

d2) Now, you can do the DECRYPTER? Pass the ENCRYPTED message (SLKAYB) and returns SKYLAB.

**Hint:** for decrypt, only catch the pair words like: **S** L **K** A **Y** B
 , then, you get SKY, the next step is catch the odd words, S **L** K **A** Y **B**, group the two groups and you get the original word.

d3) Group the **Encrypt** and **decrypt** functions in one unique function, pass the word SKYLAB and returns SKYLAB (with all the transformation inside...)

d4) **You got it?** Then try now with SKYLABCODERS. Change the function for can accept more large words.
