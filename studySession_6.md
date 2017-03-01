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
- A message will be displayed *welcoming the user*,
- The user can see a *list of flights* in a simple but comfortable message,
- The user can know which is the *most expensive* flight and which is the *cheapest*,
- What is the average price of flights for today,
- How many flights have *stopovers*,
- And knowing that the *last 5 IDs* are the last flights of the day, shows the user the last destinations (only the name)

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

---

3) BINGO GAME! 1/03 - 8/03 🎲🎰

Make a Bingo game.

The user must introduce it's name and the program make a salute.
The program, in first turn, must show a card with random numbers without repeats, distributed in five columns by three rows, each turn a ball is taught with other random number, if the number displayed matches any of the card, change the number of card matched to "X" or 0 and show again the card with the matched numbers changed at the end of turn, say to user how much numbers are matched to now.

The program should ask to user if wants continue with next turn or ends the game, if user continue, showing one different number every turn. Finally, display a message when all **ROW** is matched. **LINE X MATCHED!**

Of course, when all card numbers are matched the program should say **BINGO** and finish the game.

When the game is over, the program should say in how much turns you completed the game.
Ask to user, when the game is over, if wants play again.

**Pro** 👊🏼
- If user say 'play again', ask the name again...
- Ask to user, when the card is showed, if really wants this card or wants generate other, continue with game when user say 'yes'.
- Establish a points system, if the game ends in less turns, more points(at your decision)! If the luck is not at your side... less points :(
- Before starts the game, show to user the System points and ask to user if proceed to start the game.
- Ranking of users.
- Show the top 3 user with higher points
- Show how much games played every user.

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





