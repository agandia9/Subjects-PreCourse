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
:angry: This exercises only can be do with **METHODS**

---


### Strings
a) Hello again! I don't remember you'r name, you can tell me again please?
Write your name and count how much letters have
```javascript
console.log(myName) // My Name has 4 letters 
```

b) In what position is you'r first lastname??
```javascript
console.log(myString)// Your first last name is on position 5
```
 
c) Now, show for console **ONLY** your nane 
```javascript
console.log(myString) // My Name is Tony 
```
 
d) Now, your second lastname 
```javascript
console.log(myString) // My lastname is Stark
```
 
e) Now, replace your *name* for "Mr/Ms" and show the lastname as same 
```javascript
console.log(myNewString) // Hello, Mr. Stark 
```
 
f) Now, select your first lastname and converts to Upper Case
```javascript
console.log(mySelection) // my lastname is STARK
```

g) Now, add one message in other string var and join to other name string, show it for console
```javascript
var something = myNameVar + "is awesome"
console.log(something) \\ "Tony is awesome"

```

h) Now, you can select the first letters of your lastnames and show they?
```javascript
console.log(myFirstLastnameLetters) // S.Y
```

### Arrays
a) Declare your complete name, and print ONLY your name saparated each letter by "/"
```javascript
console.log(myName) // T/O/N/Y
```

b) Now catch your lastname and show every letter separated by "|"
```javascript
console.log(myLastName) // S|T|A|R|K
```

c) Declare your name again as a string and and show the letters with the position
```javascript
console.log(myName) // 1º T, 2º O, 3º N, 4º Y
```
Resource: https://www.w3schools.com/jsref/jsref_split.asp

d)Now, with all your name, like last exercise, show me the lastname with the position too
```javascript
console.log(myLastName) // 5º S, 6º T, 7º A, 8º R, 9º K
```
Resource: https://www.w3schools.com/jsref/jsref_length_array.asp

e) You can show me your initial letters? Like the **exercise h** in strings seccion, but with arrays 
```javascript
console.log(myInitials) // T.S
```

f)Now, introduce to array your age and print only your name and your age.
```javascript
console.log(mySelector) // My name is TONY and i'm 40 years old
```

g) Now prepare a function for introduct a city in your array, display a message with all content of array.
```javascript
console.log(myCityAdd) // City added to array! => Tony, Stark, 40, New York
```

h) Prepare other function for delete the city and asure the changes
```javascript
myCityAdd() // City added to array! => Tony, Stark, 40, New York
myCityDelete() // City deleted! => Tony, Stark, 40
```

j)Now, delete the name (first element) and asure the changes
Resources: https://www.w3schools.com/jsref/jsref_shift.asp

k) I want to introduce again my name but if I do push the name goes to last position... how I can introduce it in first position again?!
Resources: https://www.w3schools.com/jsref/jsref_splice.asp

l) Finally, declare a array from 0 to 10 and show me every element * 2
```javascript
var numbers = [0,1,2,3,4,5,6,7,8,9]
function num (num1){
    return num1 * 2
}
var mult1 = numbers.map(num)
```
Resource: https://www.w3schools.com/jsref/jsref_map.asp

m) Now, show me the new array in descending order.
Resources: https://www.w3schools.com/jsref/jsref_sort.asp

### Numbers
a) What time is it? Converts it to string and show it for console
```javascript
console.log(myString + myNumberStringify) // I'ts 10.34 of morning
```

b) What time is it exactly? Show it without the minutes.
```javascript
console.log(myString) // It's around 10 of morning
```

c) Now, try to convert your hour var with minutes to entire number without minutes and show it
```javascript
console.log(parse...(10.34)) // 10!
```

d) We can do a calculator, so let's do it! first, do a sum with two numbers
```javascript
console.log(sum) //The sum of 7+3 is 10
```

d1) Add the rest...
```javascript
console.log(sum + rest) // The sum and rest of 7 and 3 is 10 and 4 
```

d2) And the multicity
```javascript
console.log(sum + rest + mult) // 10, 4 and 21
```

d3) Finally, the division
```javascript
console.log(sum + rest + mult + div) // 10, 4, 21 and 2.3
```

d4) Now, try to execute a multiplicity like 10 * "hour", what value is returned?
```javascript
console.log(10*"hour") // ....?!
```

e) Don't worry, we can catch this error, you can controle it with **if conditional**?
```javascript
console.log(10*"hour") // You can't do this operation!
```

f) With other conditional, returns other operation
```javascript
console.log(10) // I return the same value...
```



