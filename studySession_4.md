<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">
## Challenges!

a) **FINAL!**We turn back to numbers...
So, we want do a programm that execute the Fibonacci serie
https://www.mathsisfun.com/numbers/fibonacci-sequence.html

Hint_
```javascript
function fibo(){}
// output: 0 1 1 2 3 5 8...
```

a2) You can add the position of all sums?

a3) Now, insert all results in array and show to the user

a4) Now the user should be abble to specify the position number of fibo serie it wants to see.

Hint_
```javascript
function fibo(10){}
//... 55 - pos 10º
```

a5) Now show the results in a pyramid, like:
```javascript
function fiboPymamid(num){}
0 
0 1 
0 1 1
0 1 1 2
0 1 1 2 3
0 1 1 2 3 5
0 1 1 2 3 5 8 //To pos. num
0 1 1 2 3 5 
0 1 1 2 3
0 1 1 2
0 1 1
0 1 
0
```

b) **Simple Scripting program**. Create a program that transform a 4 number values code to diferents positions, making a new code.
```javascript
var code = 3712;
function codeScript(code){}
//output:
:point_down: //First call to codeScript()
- 7123
:point_down: //Second call to codeScript()
- 1237
:point_down: //Third call to codeScript()
- 2371
// At Four call, should return the original value
```
**The first number, go to the last position. Second, third and four goes up.**

b2) Now, the user can introduce two different codes and should return the codes changed.
```javascript
function codeScript(code1, code2){}
```

b3) Now, we try to add a additional level of security. After change the position of numbers, we can multiplicy the values by 2.
*(we have a problem if the mult of numbers is > 10, choose numbers < 4 for make the code)*.
For asure the implementation of extra security level, do the properly console.logs().

b4) Now, do the DECRYPT function, call it before ends the codeScript function for asure the functionallity.
```javascript
function codeScript(code1, code2){... codeDecrypt(code1,code2)}
```


c) **Super-Challenge!!**
Create a program that use the Roman form for encrypt messages, how is that? Simple. If you have SKYLAB, the encrypted form is  SLKAYB...
If you divided the word in two groups of 3 letters, you get:
- SKY
|-|-|
- LAB 
Then, join the S with L, K with A and Y with B, and you get SLKAYB.

So, make a program that, receive the message SKYLAB and returns the SLKAYB.

c2) Now, you can do the DECRYPTER? Pass the ENCRYPTED message (SLKAYB) and returns SKYLAB.

**Hint:**: for decrypt, only catch the pair words like: **S** L **K** A **Y** B
 , then, you get SKY, the next step is catch the odd words, S **L** K **A** Y **B**, group the two groups and you get the original word.

c3) Group the **Encrypt** and **decrypt** functions in one unique function, pass the word SKYLAB and returns SKYLAB (with all the transformation inside...)

c) **You got it?** Then try now with SKYLABCODERS. Change the function for can accept more large words.
