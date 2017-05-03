<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">

## Challenges Study Sessions
 
**Mini-Proyecto de la <a href="studySession_methods.md"> primera sesión de estudio </a>**

Calculator! ➗➕

Haz una calculadora. Un único programa al que le pasarás dos parámetros y el usuario podrá visualizar por consola la suma, resta, multiplicación y división entre ambos números. El resultado debería ser mostrado con 3 decimales como mucho (En caso de que hubieran).
El programa debe contemplar y actuar correctamente en el caso de que el usuario introduzca cualquier cosa que no sean números.

Como objetivos extra:

- Si el usuario introduce un solo numero, deberá mostrar **SOLO** su raíz cuadrada, si vuelve a introducir los dos, volverá a mostrar las 4 operaciones de siempre.
- Los resultados deberían almacenarse dentro de una array y mostrarlos de una forma amigable al usuario.

*Hint_* => results = [num1 + num2 = resultSum, num1-num2 = resultRest ....]

**PRO.**

- Podrías hacer que le calculadora relizara operaciones sean cuales sean el numero de argumentos pasados a la funcion?
*Hint* => https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/arguments
*Hint* => https://msdn.microsoft.com/es-es/library/he95z461
```javascript
function sum(){
    var acc = 0;
    for (num in arguments){
    console.log(num)
    acc += arguments[num]   
    } 
    return acc
}
sum(2,3,4) // acc=9
```

- Después de hacer todas las operaciones, el programa deberá preguntar al usuario si desea volver a realizar otra operación, volviendo a almacenar más resultados y mostrándolos.
```javascript
calculator(n1,n2)
//Output => sum, subs, mult, div...
prompt("New numbers? y/n")
    Case "y" => calculator(n1,n2)
                //Output => sum1, subs1, mult1, div1, sum2, subs2, mult2, div2...
    Case "n" => "Bye!"
```

---

**Mini-Proyecto de la <a href="studySession_objects.md"> segunda sesión de estudio </a>**

Skylab Airlines! ✈️🛩

*(Los datos están al final del enunciado, podéis usarlos en vuestro código)*
Programa una inferfaz de usuario para una aerolinea. Esta aerolinea dispondrá de 10 vuelos para el dia de hoy, para empezar, estos vuelos estarán declarados de manera global, cuando se llame a la función:
- Se preguntará por el nombre de usuario y dará la bienvenida.
- El usuario visualizará todos los vuelos disponibles de una forma amigable:
    El vuelo con origen: *Barcelona*, y destino: *Madrid* tiene un coste de *XXXX€*  y no realiza *ninguna* escala.
- A continuación, el usuario verá el coste medio de los vuelos.
- También podrá ver cuantos vuelos efectúan escalas.
- Y, sabiendo que los ultimos 5 vuelos (los últimos 5 ID's) son los últimos del día, muestra al usuario sus destinos.

**PRO!:**

Después de ver toda la información el programa pedirá al usuario si es ADMIN/USER, dependiendo de la elección, el programa se comportará de la siguiente manera: 

Si eres *ADMIN*, la función debería permitir:
- Poder crear, más vuelos, pidiendo la información por prompt(), sin poder pasar de 15 vuelos, si se intenta introducir uno más, saltará un alert().
- Poder eliminar vuelos mediante el ID.

Si eres *USER* la función debería permitir:
- Buscar por precio ( más alto, más bajo o igual), el usuario debería mostrar los datos de los vuelos encontrados y, indicando el ID, el programa responderá:
"Gracias por su compra, vuelva pronto."


_Resources:
http://stackoverflow.com/questions/1290131/javascript-how-to-create-an-array-of-object-literals-in-a-loop

http://stackoverflow.com/questions/15742442/declaring-array-of-objects


```javascript
// This is a example of array of objects... each position of array contains one object...
var flights = [
{id: 00, to: "New York", from: "Barcelona", cost: 700,scale: false},
{id: 01, to: "Los Angeles", from: "Madrid", cost: 1100,scale: true},
{id: 02, to: "Paris", from: "Barcelona", cost: 210,scale: false},
{id: 03, to: "Roma", from: "Barcelona", cost: 150,scale: false},
{id: 04, to: "London", from: "Madrid", cost: 200,scale: false},
{id: 05, to: "Madrid", from: "Barcelona", cost: 90,scale: false},
{id: 06, to: "Tokyo", from: "Madrid", cost: 1500,scale: true},
{id: 07, to: "Shangai", from: "Barcelona", cost: 800,scale: true},
{id: 08, to: "Sydney", from: "Barcelona", cost: 150,scale: true},
{id: 09, to: "Tel-Aviv", from: "Madrid", cost: 150,scale: false}
]
console.log(flights[0].to) //output: New York
```

---

**Mini-Proyecto de la <a href="studySession_functions.md"> tercera sesión de estudio </a>**


BINGO GAME! 🎲🎰

Realiza un programa que simule un Bingo. Cuando se ejecute, pedirá el nombre del jugador y deberá guardarse. Durante el primer turno se mostrará un cartón con 15 números (excluyendo el 0 siempre), y cada turno, otro número se visualizará, si coincide con alguno de los existentes en el cartón, cambiará por una "X" o un 0. El cartón se mostrará, al final de cada turno, con los cambios efectuados, indicándole al usuario qué número se ha encontrado.
El programa deberá preguntar al usuario al inicio de cada turno si desea continuar, en caso de que se continúe, seguirá el mismo patrón que hasta el momento.

Por supuesto, cuando todos los números de una misma linea estén en "X", mostrará un mensaje "LINEA!", pero la ejecución seguirá, el juego solo acabará cuando todos los números estén a "X".

Cuando el juego concluya, deberá decirle al usuario en cuantos turnos se ha completado el cartón. Por último, deberá preguntar si desea volver a jugar.

**Pro** 👊🏼
- Cuando se muestre la carta, se preguntará al usuario si realmente quiere ese cartón o generar otro, si realmente quiere ese cartón, deberá responder "yes" para proceder
- Establece un sistema de puntos, en cuantos más turnos se complete el cartón, menos puntos (el sistema de puntos intégralo como quieras), por el contrario, a menos turnos, más puntos.
- Antes de empezar el juego, muestra el sistema de puntos al usuario.
- Ranking de usuarios (ordenado por puntos).

Resources_
http://dlevin.pcprofessor.net/javaScript/bingo/bingo.html
https://www.w3schools.com/jsref/jsref_random.asp

Hint_
```javascript
var bingoCard = [
    {number: randomNumber, matched: false},
    {number: randomNumber, matched: false},
    {number: randomNumber, matched: false},
    {number: randomNumber, matched: false},
    {number: randomNumber, matched: false},
    //next line
    {number: randomNumber, matched: false},
    {number: randomNumber, matched: false},
    {number: randomNumber, matched: false},
    {number: randomNumber, matched: false},
    {number: randomNumber, matched: false}
]
```

---

**In reference to 4º Study Session**

Pasapalabra Game! (Final JS) 🎮⁉️

Resource: https://www.youtube.com/watch?v=xJp2c_rcHDc
Haz el juego del Pasapalabra, el programa deberá lanzar preguntas relacionadas con una palabra y el usuario deberá responder con esa misma palabra, por ejemplo:

```
'>>>'With the letter "A", if is not a person... is?
'>>>' "Animal"
'>>>'Correct, you have 1 Point!
```

Entonces, tu juego debería hacer una pregunta por letra del alfabeto, al final del juego, y habiendo respondido **todas las letras**, deberá indicarle al usuario cuantas letras ha fallado y cuantas ha acertado.
Si el usuario responde con "pasapalabra" el juego deberá estar preparado para entender que en ese momento, el usuario no responderá esa pregunta, y no estará acertada ni fallada, la dejará para la siguiente ronda.
El juego deberá, cuando finalize, mostrar un ranking de usuarios con el nombre y ordenados por cantidad de letras acertadas.

**PRO**
- Los usuarios deberán tener tiempo límite por cada juego, por ejemplo 130 segundos...
*Resource*: https://www.w3schools.com/jsref/met_win_settimeout.asp
- El programa no debería hacer distinciones entre mayúsculas, minúsculas... 
*Ejemplo*: **"animal" == "ANIMAL" // "Animal" // "aNiMal"...**
- El programa debe estar preparado para aceptar el input "END" para terminar el juego en cualquier momento, si esto sucede, el programa dirá cuantas letras ha acertado pero no entrará en el ranking.
- Prepara tu programa para que no repita siempre las mismas preguntas, por ejemplo, de la misma letra, se podrían hacer tres preguntas diferentes.




