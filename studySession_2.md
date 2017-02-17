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
console.log(student.name) // "David Aughan"
```

*Working with objects*
#### Reference:
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects

---

### 3...2...1...GO!

a) Do a simple function for show the names of the properties. 
```
console.log(something, somethingMore, somethingMoreAndMore)
//name, class, id
```

b) Now, do a simple function for show the **content** of those properties.
```
console.log(somethingThatShowsThings) //Tony, VII, 01
```

c) So, we can change a property value? Change the class to "XI".
```
console.log(property.ThisProperty) //new value
```

d) Now, delete the id property.
```
console.log(property.ThisProperty) //Not exist :(
```

e) Add a new property called **city** and give some value

http://www.w3schools.com/js/js_properties.asp

e1) Asure the changes showing the property in console.
```
console.log(city) // New York City
```

f) List the number of properties we have now on objects.
```
console.log() // There are 4 info fields
```

g) Change the property **name** to **fullName**

g1) Asure the changes.
```
console.log(fullName) // Tony Stark
```

h) For last, add a presentation message like: "Hello, my name is " + ..., and show all values of the object.
```
console.log(...) // "Hi there, I'm Tony Stark..."
```

h1) Add some properties more...like job, Studies and Marks average

h2) Asure the changes and show for console.

```
console.log(location) // NYC
```

i) Make a **constructor** object called avenger and pass the info, creating a instance of the object with the properties of our created object

http://www.w3schools.com/js/js_object_definition.asp

Example:

```
function avenger(fullName, class, city, job, studies,markAv) {
    this.fullName = fullName;
    this.class = class;
    this.city = city;
    this.job= job;
    this.studies= studies;
    this.markAv = markAv;
}
var tonyStark = new person ("Tony Stark", "XI", "NYC", "Ingeneer", "MIT", 10)
console.log(tonyStark)
```

j) Create other avenger and print the name for console
```
var otherAvenger = new Avenger...
console.log(otherAvenger) // Hulk...
```

k) Now create one property of object that print a pretty description of avengers.
```
console.log(otherAvenger.somethingThatShows) // Hulk, 30...
```

l) Now, make a function that only shows the NAMES of created avengers.
```
console.log(someFunction) // Tony Stark, Hulk, Thor...
```

m) Make other student and prepare for ONLY show the names, the age and location.
```
console.log(propertyValues) // my name, my age and my location!
```

n) For last, create yourself and create a function for catch all averages field of Avengers and shows the average of all of them.

