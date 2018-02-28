# JS Arrays

## Setup
* Create a new repo called jsArrayChallenges
* Create a new folder ~/workspace/static-web/exercises/jsArrayChallenges
* Push up a README.md
* Setup:  make an index.html and main.js.  Index should have boilerplate and script tag.  main.js file should have console.log


## Requirements
* This assignment contains 10 challenges that involve arrays
* Each challenge should be done on a new branch - I should see 10 merged PRs to know you are done with this assignment
* For each challenge make a div with an id of that challenge number in the index.html.  
```
<div id="challenge-1"></div>
```
* The ouput for each challenge should be displayed in the coresponding div
* Before you merge each challenge in check that the code is properly indented and remove ALL console.logs

## Challenges

### Challenge #1: Highest Scoring Word
Given a string of 2 words, find the highest scoring word.  Each letter of a word scores points according to it's position in the alphabet: a = 1, b = 2, c = 3 etc. All letters will be lowercase there will be no punctuation.  Display (id='challenge-1') the word that is the highest scoring.  If two words score the same, display the word that appears earliest in the original string.

```
var challengeOneInput = "jumbo shrimp";  //jumbo=61, shrimp=83 should display shrimp
```

### Challenge #2: Sorting on planet Twisted-3-7

There is a planet... in a galaxy far far away. It is exactly like our planet, but it has one difference:  The values of the digits 3 and 7 are twisted. Our 3 means 7 and 7 means 3.

Write some code that takes an array of numbers and outputs an array that changes any 3s to 7s and any 7s to 3s.

```
var challengeTwoInputA = [1,2,3,4,5,6,7,8,9];  //[1,2,7,4,5,6,3,8,9];
var challengeTwoInputB = [12,13,14];  //[12,17,14];
var challengeTwoInputC = [9,2,4,7,3];  //[9,2,4,3,7];
```

<hr/>
### Challenge #3: Find the unique number
Given an array of more than 3 numbers where all numbers are equal except for one. Display the one unique number!
```
var challengeThreeInputA = [ 1, 1, 1, 2, 1, 1 ];  // 2
var challengeThreeInputB = [ 0, 0, 0, 0, 0, 0, 0, 0.55, 0, 0 ];  // 0.55
```

<hr/>
### Challenge #4: Lost Without a Map
Given an array of any number of integers display the array with each value doubled.
```
var challengeFourInputA = [ 1, 2, 3 ];  // [2, 4, 6]
var challengeFourInputB = [ 3, 8, 1, 2, 4, 12 ];  // [ 6, 16, 2, 4, 8, 24 ]
```

<hr/>
### Challenge #5: Array.diff
Given two arrays remove all values from array1 that are present in array2.

Example 1:
```
var array1 = [1,2];
var array2 = [1];
//display = [2]
```

Example 2:
```
var array1 = [1,2, 4, 7, 5, 9];
var array2 = [5, 9, 2];
//display = [1, 4, 7]
```

<hr/>
### Challenge #6: Number Zoo Patrol
You're working in a number zoo, and it seems that one of the numbers has gone missing!  Given an array of numbers. The numbers will be unsorted values between 1 and one more than the length of the array. No values will be repeated within the array. displaythe number that is missing.

Examples:
```
var test1 = [1,3]; // 2
var test2 = [2,3,4]; // 1
var test3 = [13,11,10,3,2,1,4,5,6,9,7,8]; // 12
```

<hr/>
### Challenge #7: English beggars
Given an array of values and an amount of beggars, you are supposed to return an array with the sum of what each beggar brings home, assuming they all take regular TURNS, from the first to the last. Not all beggars have to take the same offers - ie the length of the array is not a multiple of the number of beggers.  Dipl

Example 1:
```
var numBeggers = 2;
var offerings = [1,2,3,4,5];
// first one takes [1, 3, 5]=9
// second one takes [2, 4]=6

//display [9, 6]
```

Example 2:
```
var numBeggers = 3;
var offerings = [1,2,3,4,5];
// first one takes [1, 4]=5
// second one takes [2, 5]=7
// second one takes [3]=3

//display [5, 7, 3]
```

<hr/>
### Challenge #8: 
<hr/>
### Challenge #9: 
<hr/>
### Challenge #10: 





