<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">

## Functions

http://www.w3schools.com/js/functions.asp

*Simple JS Function for example.*

```
var x = myFunction(4, 3);

function myFunction(a, b) {
    return a * b;
}

```


a) First we can do a basically sum, you can do it? Write a function and call it for see the result
```
function(){} // 2+2=4
```

b) Then, add the rest.
```
function(){} // 2+2=4, 2-2=0
```

c) And add the multiplication and division
```
function(){} // 2+2=4, 2-2=0, ...4, ...1
```

d) Add a message that execute with this function, in this message add the result of the previous operations
```
function(){} // The results are... 
```

e) Now, try give a name to out function and call it
```
var MyFunction = ...

```

f) Now try to declare the numbers out of function and pass they as a parameter.
```
var a ...
var b ...
function(a,b)
```

g) Now, delete the numbers, how we can call this function and pass the parameters in the call? (You can delete now the message string created in exercise **d**)
```
function(a,b)...{}
myFunction(a,b);

```


h) Try to generate random numbers out of a our function and operate with they, this numbers should be passed as a parameter
```
    var randomA=...
    var randomB=...

    function calculator(randomA,randomB){
        .
        .
        .
        return something, somethingMore
    }
```

http://www.w3schools.com/jsref/jsref_random.asp

i) Now, try to return the results of the calculate function to other function and show the results

```
function callCalculator(){
    var randomA
    var randomB
    calculator(randomA,randomB){
        return something, somethingMore
    }
}
```


j) Now, try to return this results as a String for show a message.
```
function callCalculator(){
    .
    .
    .
    return string;
}
```

k) Try to catch the errors if the number passed to our calculator function is a NaN and return error if this happen.

l) And, try to catch if the number is undefined or null, and show other error as a message.

m) Let's make this a little bit more complicated... The random numbers should be generate in other diferent function.. return to our father function and passed as a parameter to our calculate function
```
function Generate(){
    ...
    return randomNumbers.
}

function father(){
    Generate();
    calculator(randomNumbers){
        .
        .
        .
    }
}
```

n) Then, for get all our program separated in functions, try to slice all functions, in the principal function you must only have the calls to this functions.
```
function father(){
    myFunction();
    myOtherFunction();
    myOtherFarFunction();
}

```

ñ) Now, try to push the results of calculator in array and pass as a parameter instead as a var like always

o) Create other function for calculate the average of all Calculator results and call it the last position, show the average just after all other callings
```
// .........And the average is X
```

p) Now, try to compare two averages, averages that you get after call two times the father function and of course, are different. Print what average is bigger.



---

