# JS Objects

## Setup
* Create a new repo on Github called jsObjectChallenges
* Create a new folder ~/workspace/static-web/exercises/jsObjecChallenges
* Push up a README.md with the title of the repo on to master branch
* Setup branch:  make an index.html and main.js.  Index should have boilerplate and script tag.  main.js file should have console.log. You should run http-server and confirm that there are no errors and that everything is working as expected.


## Requirements
* This assignment contains 10 challenges that involve objects
* Each challenge should be done on a new branch - I should see 10 merged PRs (11 total with setup) to know you are done with this assignment
* For each challenge make a div with an id of that challenge number in the index.html.  
```
<div id="challenge-1"></div>
```
* The ouput for each challenge should be displayed in the coresponding div
* Before you merge each challenge in check that the code is properly indented and remove ALL console.logs

## Challenges

### Challenge #1: Wheel of Fortune
Three candidates take part in a TV show.  In order to decide who will take part in the final game and probably become rich, they have to roll the Wheel of Fortune!The Wheel of Fortune is divided into 20 sections, each with a number from 5 to 100 (only mulitples of 5).  Each candidate can roll the wheel once or twice and sum up the score of each roll. The winner one that is closest to 100 (while still being lower or equal to 100). In case of a tie, the candidate that rolled the wheel first wins.

You receive the information about each candidate as an array of objects: each object should have a name and a scores array with the candidate roll values.  Display the name of the winner or false if there is no winner (all scored more than 100).

Examples:
```
var players = [{ name: "Bob", scores: [10, 65] }, { name: "Bill", scores: [90, 5] }, { name: "Charlie", scores: [40, 55] }]; // Displays "Bill"
var players = [{ name: "Bob", scores: [15, 20] }, { name: "Bill", scores: [10, 15] }, { name: "Charlie", scores: [90, 10] }]; // Displays "Charlie"
```

<hr/>


### Challenge #2: Find how many times did a team from a given country win the Champions League?
Given an array called winnerList and the name of a country, display the number of times a team from a given country has won. Return 0 if there have been no wins.

For example
```
var winnerList = [
  {season: '1999-2000', team: 'Real Madrid', country: 'Spain'},
  {season: '2000-2001', team: 'Bayern Munich', country: 'Germany'},
  {season: '2001-2002', team: 'Real Madrid', country: 'Spain'},
  {season: '2002-2003', team: 'Milan', country: 'Italy'},
  {season: '2003-2004', team: 'Porto', country: 'Portugal'},
  {season: '2004-2005', team: 'Liverpool', country: 'England'},
  {season: '2005-2006', team: 'Barcelona', country: 'Spain'},
  {season: '2006-2007', team: 'Milan', country: 'Italy'},
  {season: '2007-2008', team: 'Manchester United', country: 'England'},
  {season: '2008-2009', team: 'Barcelona', country: 'Spain'},
  {season: '2009-2010', team: 'Internazionale', country: 'Italy'},
  {season: '2010-2011', team: 'Barcelona', country: 'Spain'},
  {season: '2011-2012', team: 'Chelsea', country: 'England'},
  {season: '2012-2013', team: 'Bayern Munich', country: 'Germany'},
  {season: '2013-2014', team: 'Real Madrid', country: 'Spain'},
  {season: '2014-2015', team: 'Barcelona', country: 'Spain'},
  {season: '2015-2016', team: 'Real Madrid', country: 'Spain'},
  {season: '2016-2017', team: 'Real Madrid', country: 'Spain'},
];
var country = 'Spain'  // should return 8
var country = 'Portugal'  // should return 1
var country = 'Russia'  // should return 0


```

<hr/>


### Challenge #3: Arithmetic
Given an object containing two numbers and an arithmetic operator, return the appropriate math result..

The four operators are "add", "subtract", "divide", "multiply".

A few examples:
```
var test1 = {a: 5, b:2, operator: "add"};  //7
var test1 = {a: 5, b:2, operator: "subtract"}; //3
var test1 = {a: 5, b:2, operator: "multiply"}; //10
var test1 = {a: 5, b:2, operator: "divide"}; //2.5
```

<hr/>


### Challenge #4: Ziiiiip!
Let's implement the zipObject function that takes and array of names and an array of ages and smashes them into one object.


Example:
 ```
var names = ['fred', 'barney'];
var ages = [30,40];
//Output:  { 'fred': 30, 'barney': 40 }
```

<hr/>


### Challenge #5: Strive Matching
The company Strive is looking for a new developer.  Given a candidates minSalary and a jobs maxSalary determine if the company can affort the candidate.  The Company will only accept candidates that have a minSalary that is at least 10% less than the jobs maxSalary.  If the candidate matches display true otherwise display false.

Examples:
```
var candidate1 = {
  minSalary: 120000
};
let job1 = {
  maxSalary: 140000
}
//output is true.  this job can hire any minSalary less than 126,$000


var candidate1 = {
  minSalary: 950000
};
let job1 = {
  maxSalary: 100000
}
//output is false.  this job can hire any minSalary less than 90,$000
```
