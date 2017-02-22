<img src="http://www.skylabcoders.com/images/403/default.png" alt="Skylab" style="width:200px;height:45px;">

## Challenges Study Sessions
 
1) Calculator! 15/02 -> 21/02➗
Make a calculator, a single function program to which you will pass two numbers, and will display by console its sum, subtraction, multiplication and division. The results should be shown only with 3 decimals at most (if exist...) and contemplate that if, the user enters anything other thing than numbers, it should show an error

As EXTRA objectives:

- In addition, to be able to make square roots
- Prepare the function for can accept more than 2 parameters...
- Show results by storing them in an array along with the operands:

*Hint_* => results = [num1 + num2 = resultSum, num1-num2 = resultRest ....]

**PRO.**
-After do all operations, ask to user if wants make other operation with other numbers, the array should storage the results of first execution and second.
Good luck!

---

2) Skylab Airlines! 22/02 - 28/02 ✈️🛩
Make the **interface of an airline**, this airline has 10 flights available for today (In object format), to begin with, flights are declared globally, when the function is called...:
. A message will be displayed *welcoming the user*,
. The user can see a *list of flights* in a simple but comfortable message,
. The user can know which is the *most expensive* flight and which is the *cheapest*,
. What is the average price of flights for today,
. How many flights have *stopovers*,
. And knowing that the *last 5 IDs* are the last flights of the day, shows the user the last destinations (only the name)

**PRO!:**

You must indicate to the function if you are admin or user. 

If you are *admin* the function, through the user prompt, you should:
- To be able to *create more flights*, up to 15, when the number of flights reaches 15, must show the error that the airport have collapsed.
- *Delete* flights by ID

If you are a *user*:
- You can s*earch for price*, higher, less or equal, a question will be displayed indicating which flight you want, *indicating the ID*, will show the selected flight information and a message: Thank you for your purchase, good day!
- Ask to user if you want *make other purchase*, directly, asking by the ID of the new flight

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




