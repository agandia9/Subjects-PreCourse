<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">

## JS Objects{😎}

#### Reference:

http://www.w3schools.com/js/js_objects.asp

*Simple JS Object for example.*

```javascript
var avenger = { 
    name : "Tony", 
    class : "VII", 
    id : 1 
};
console.log(student.name) // "David Aughan"
```

*Working with objects*
#### Reference:🤓
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects

http://javascript.info/tutorial/objects

https://www.w3.org/wiki/Objects_in_JavaScript //Try to do the exercise of calculate the area of triangle 

---

a) Escribe una función que liste los nombres de propiedad del objeto 
(Puedes usar el objeto creado más arriba)
```javascript
console.log(something, somethingMore, somethingMoreAndMore)
//name, class, id
```

b) Ahora, crea una función que liste solo los valores de las propiedades.
```javascript
console.log(somethingThatShowsThings) //Tony, VII, 01
```

c) Cambia el valor de la propiedad class por "XI" y asegurate de que los cambios se han efectuado.
```javascript
console.log(property.ThisProperty) //new class = XI
```

d) Ahora, elimina la propiedad ID y asegura los cambios.
```javascript
console.log(property.ThisProperty) //Not exist :(
```

e) Añade una nueva propiedad, por ejemplo **city** y dale un valor.

http://www.w3schools.com/js/js_properties.asp

e1) Asegura los cambios solo imprimiendo esa nueva propiedad.
```javascript
console.log(city) // City => New York City
```

f) Lista el numero de propiedades que contiene el objeto.
```javascript
console.log() // There are 4 info fields
```

g) Cambia la propiedad **name** por **fullName**.

g1) Asegura los cambios.
```javascript
console.log(fullName) // Tony Stark
```

h) Lista todas las propiedades del objeto a través de un console.log()
```javascript
console.log(...) // "Hi there, I'm Tony Stark..."
```

h1) Añade más propiedades al objeto, como... markAverage, country, job, studies...

h2) Asegura los cambios volviendo a listar los valores del objeto

```javascript
console.log(location) // NYC
```

i) Crea un **constructor** de objetos llamado "Avenger", al cual le pasarás ciertos parametros, creando una instancia del objeto con las propiedades de nuestro objeto creado.
(Échale un ojo a la referencia de abajo.) 

http://www.w3schools.com/js/js_object_definition.asp

Example:

```javascript
function avenger(fullName, classRoom, city, job, studies,markAv) {
    this.fullName = fullName;
    this.classRoom = classRoom;
    this.city = city;
    this.job= job;
    this.studies= studies;
    this.markAv = markAv;
}
var tonyStark = new avenger ("Tony Stark", "XI", "NYC", "Ingeneer", "MIT", 10)
console.log(tonyStark)
```

j) Crea otro objeto y imprime sus propiedades por pantalla.
```javascript
var otherAvenger = new Avenger...
console.log(otherAvenger) // Hulk...
```

k) Crea una propiedad del objeto que liste automáticamente los valores de la instancia.
Example of property:
```javascript
this.listProperties: function(){
    console.log(this.name + ", " + this.class) 
};
```

<details> 
  <summary>Spoiler! 😅</summary>
  <div>
```javascript
function avenger(fullName, classRoom, city, job, studies,markAv) {
    this.fullName = fullName;
    this.classRoom = classRoom;
    this.city = city;
    this.job = job;
    this.studies = studies;
    this.markAv = markAv;
    this.description = function(){
        console.log(this.fullName + ", " + this.city + "...")
    }
}
var tonyStark = new avenger ("Tony Stark", "XI", "NYC", "Ingeneer", "MIT", 10)
tonyStark.description()
//Tony Stark, NYC...
```
</div>
</details>


l) Ahora, crea una función que solo liste los nombres de los objetos instanciados
```javascript
console.log(someFunction) // Tony Stark, Hulk, Thor...
```

m) Crea varios objetos con las mismas propiedades, como por ejemplo la ciudad, crea una función para que **solo liste los nombres** de los Avengers **que sean de la misma ciudad** y cuantos hay.
```javascript
console.log(myFunction) // Are 3 avengers living in NYC: Tony, Hulk, Hawkeye
```

n) Para acabar, créate a ti mismo y crea una función que recoja todas las markAv y muestre la media de todas las notas.

ñ) Ahora, crea una funcion que recoja los avengers en parejas (será necesario que tengan un id...), es decir, de dos en dos, compare sus markAv y que solo muestre el mayor.
```javascript
console.log(myFunction()) // HawkEye vs Tony => Tony is better! \n Thor vs Hulk => Hulk is better! \n Vision vs Captain America => Vision is better
```
