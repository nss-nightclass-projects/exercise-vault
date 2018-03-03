# JS Functions

## Setup
* Create a new repo on Github called jsFunctionChallenges
* Create a new folder ~/workspace/static-web/exercises/jsObjecChallenges
* Push up a README.md with the title of the repo on to master branch
* Setup branch:  make an index.html and main.js.  Index should have boilerplate and script tag.  main.js file should have console.log. You should run http-server and confirm that there are no errors and that everything is working as expected.
* Write a function called writeToDom that takes two inputs - domString and domId.  This function should use the domId to grab the output div and write the domString to it for example:
```
writeToDom("I go in div#2", "challenge-2");

writeToDom(domString domId){
  <DO STUFF HERE to put "I go in div#2" in the div is id="challenge-2">
}


```


## Requirements
* This assignment contains 5 challenges that involve functions
* Each challenge should be done on a new branch - I should see 10 merged PRs (11 total with setup) to know you are done with this assignment
* Once you have an answer use the writeToDom function that you created when you did the setup branch to display the result
* Before you merge each challenge in check that the code is properly indented and remove ALL console.logs

## Challenges

### Challenge #1: How old will I be in 2099?
Philip's just turned four and he wants to know how old he will be in various years in the future such as 2090 or 3044. His parents can't keep up calculating this so they've begged you to help them out by writing a programme that can answer Philip's endless questions.

Your task is to write a function that takes two parameters: the year of birth and the year to count years in relation to. As Philip is getting more curious every day he may soon want to know how many years it was until he would be born, so your function needs to work with both dates in the future and in the past.

Provide output in this format: For dates in the future: "You are ... year(s) old." For dates in the past: "You will be born in ... year(s)." If the year of birth equals the year requested return: "You were born this very year!"

Examples:
```
challenge1(2000, 2010); // You are 10 years old.
challenge1(2000, 1995); // You will be born in 5 years.
challenge1(2000, 2000); // You were born this very year!
```

<hr/>


### Challenge #2: Simple Maths Test
Create a function which checks a number for three different properties.

1.  Is the number prime?
2,  Is the number even?
3.  Is the number a multiple of 10?
Each should return either true or false, which should be given as an array.

Examples:

```
challenge2(7)  // ==> [true,  false, false] 
challenge2(10) // ==> [false, true,  true]
```

<hr/>


### Challenge #3: Unique Sum
Given a list of integers values, your job is to return the sum of the values; however, if the same integer value appears multiple times in the list, you can only count it once in your sum.

For example:
```
challenge3([ 1, 2, 3]) //6
challenge1([ 1, 3, 8, 1, 8]) //12
challenge1([ -1, -1, 5, 2, -7])//-1
```

<hr/>


### Challenge #4: Filter out the geese
Write a function that takes an array of strings as an argument and returns a filtered array containing the same elements but with the 'geese' removed.

The geese are any strings in the following array:
```
geese = ["African", "Roman Tufted", "Toulouse", "Pilgrim", "Steinbacher"]
```
Example:
```
challenge4(["Mallard", "Hook Bill", "African", "Crested", "Pilgrim", "Toulouse", "Blue Swedish"]) //["Mallard", "Hook Bill", "Crested", "Blue Swedish"]
```

<hr/>


### Challenge #5: Sort by Last Char
Given a string of words (x), you need to return an array of the words, sorted alphabetically by the final character in each.

If two words have the same last letter, they returned array should show them in the order they appeared in the given string.

challenge5("I love pie"); //["love", "pie", "I"]
challenge5("bears live in the woods"); //["live", "the", "in", "bears", "woods",]
