<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">
## JS Objects
####Reference:
http://www.w3schools.com/js/js_objects.asp

*Simple JS Object for example.*

```
var student = { 
    name : "David Aughan", 
    class : "VI", 
    id : 12 
};

```

*Working with objects*
#### Reference:
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects

---

### 3...2...1...GO!

a) Do a simple function for show the names of the properties. 
output: name/class/id
```
console.log(something, somethingMore, somethingMoreAndMore)
//Tony, VII, 01
```

b) Now, do a simple function for show the **content** of those properties.
```
console.log(somethingThatShowsThings) //Tony, VII, 01
```

c) So, we can change a property value? Change the class to "XI".
```
console.log(property.ThisProperty) //NewProperty
```

d) Now, delete the id property.
```
console.log(property.ThisProperty) //Not exist :(
```

e) List the number of properties we have now on objects.
```
console.log() // There are 4 info fields
```

f) Add a new property called **city** and give some value

http://www.w3schools.com/js/js_properties.asp

f1) Asure the changes showing the property in console.
```
console.log(city) // New York City
```

g) Change the property **name** to **fullName**

g1) Asure the changes.
```
console.log(fullName) // Tony Stark
```

h) For last, add a presentation message like: "Hello, my name is " + student.name....., and show all values of the object.
```
console.log(...) // "Hi there, I'm Tony Stark..."
```

h1) Add some properties more...like Location, Studies and Marks average

h2) Asure the changes and show for console.

```
console.log(location) // NYC
```

i) Make a **constructor** object called Student and pass the info, creating a instance of the object with the properties of last object

http://www.w3schools.com/js/js_object_definition.asp

Example:

```
function person(first, last, age, eye) {
    this.firstName = first;
    this.lastName = last;
    this.age = age;
    this.eyeColor = eye;
}
var myFather = new person("John", "Doe", 50, "blue");
var myMother = new person("Sally", "Rally", 48, "green");
```

j) Create other student and print the name for console
```
var otherAvenger = new Avenger...
console.log(otherAvenger) // Hulk
```

k) Now create one property of object that print a description of students.
```
console.log(otherAvenger.somethingThatShows) // Hulk, 30...
```

l) Now, change description property of constructor object and prepare for show the info about the student

m) Make other student and prepare for ONLY show the names, the age and location.
```
console.log(propertyValues) // my name, my age and my location!
```

n) For last, create yourself as a student using the constructor object

