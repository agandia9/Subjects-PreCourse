<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">

## Functions JS

_Resources to check:

- http://www.w3schools.com/js/functions.asp
- http://helephant.com/2008/08/23/javascript-anonymous-functions/
- https://teamtreehouse.com/community/why-call-consolelog-on-a-function-when-its-already-logged-to-the-console-seems-redundant-same-effect
- http://stackoverflow.com/questions/21020608/difference-between-console-log-and-return-in-javascript

*Simple JS Function for example.*

```javascript
var x = myFunction(4, 3);

function myFunction(a, b) {
    return a * b;
}

var y = function myFunction(a, b) {
    console.log(a * b)
}

```


a) First we do a function that salute us, try to pass your name as param of function and print out for console.
```javascript
console.log('hello + myName')//output: 'hello myName'
```

b) Try to RETURN this same values instead of console.log()
```javascript
return 'hello + myName' // output: 'hello myName'
```

c) Now, add your age and **return** it with your name too.

```javascript
return 'myMessage' //output: 'hello myName, you're myAge years old.'
```

d) Equal your function to one var and execute it.
```javascript
var MyFunction = ... //output: 'hello myName, you're myAge years old.'

```

e) Now, try to declare other function and assign it result to other variable called myAge, and try to print the result of both functions in one line.
```javascript
myName() + myAge() //output: IronMan 40
```

f) Now try to declare the vars and pass as a parameter.
```javascript
var...
var...
myName(param1) + myAge(param2) //output: IronMan 40

```

g) Try to englobe in one function both vars and execute it, the output should be the same.

```javascript
function ... (){
    var x = myName(param1)
    var y = myAge(param2)
    return x + y
} //output: IronMan 40
```


h) Try to generate random numbers in other function and pass as parameter to function that return the age.
```javascript
return x + y // output: IronMan 6457689
```

http://www.w3schools.com/jsref/jsref_random.asp

i) Now, limit the random from 0 to 50. Say one message if the output age is < 20 and other if > 21
```javascript
return x + y // output: IronMan 3...Sure you're Tony Stark?
```

j) Now, the function that receive the name, modify it and concatenate one string to the random num and return both
```javascript
return x + y // output: Tony Stark...aka IRONMAN, 34...Sure you're Tony Stark? 
```


k) Now, change the return of the father function for console.log and show both child functions returns in pretty string
```javascript
return x + y // output: The first function returns: 'Tony Stark...aka IRONMAN', The second function returns: '34...Sure you're Tony Stark?' 
```

l) Try to catch the error if the Name passed to our child function... if is not IronMan, show message.
```javascript
return x + y // output: The first function returns: 'Tony Stark...aka IRONMAN', The second function returns: '34...Sure you're Tony Stark?' 
```


m) Let's make this a little bit more complicated... The random numbers should be generate in other diferent function.. return to our father function and passed as a parameter to our second function
```javascript
function GenerateRandom(){
    ...
    return randomNumber.
}
function father(){
    GenerateRandom();
    return x()...
}
```

n) Then, for get all our program separated in functions, try to slice all functions, in the principal function you must only have the calls to this functions.
```javascript
function father(){
    myFunction();
    myOtherFunction();
    myOtherFarFunction();
}

```

ñ) Now, try to push the results of callfunctions in array and return one string like always

o) Create other function that call to our father function, this separated function uses the array of results and push other string like: I'M CALLED FROM THE OTHER SIDE!!

p) Now, try to call this function to times, what random Num of those two calls is bigger? 



