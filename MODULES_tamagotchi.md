# Tamagotchi
Remember Tamagotchi's?  They looked something like this:

![Tamagotchi](./images/tamagotchi.jpg)

In case you lived under a rock in the 90s a Tamagotchi was the first "digital virtual pet".  It had three buttons and 8 different menus.  After activating it an egg would hatch and then you would be responsible for keeping your pet alive.  Your pet could do things like eat, sleep, play, get sick, get medicine, and poop.  They sold over 82 million of them before 2017.

For this HW we are going to create a simplified version of a Tamagotchi.

If you are worried you version will never be as good as the original you can still buy yourself a real one [HERE](https://www.bandai.com/tamagotchi/)

## Setup
This project will be built with modules that are laced together with webpack.  Set up webpack, eslint, and babel like we have done in class.

## Styling
You may **NOT** use bootstrap or any styling framework for this project.

All your styling should be in files that end in `.scss`.  At minimum you should be using SASS variables and nesting.  But I challenge you to dig into the [SASS Guide](https://sass-lang.com/guide) and use some of the other cool sass tools.

## HTML
Your index.html file should look like this:
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Tamagotchi</title>
</head>
<body>
  <div id="app">
    <div id="progress"></div>
    <div id="eat" class="quad"></div>
    <div id="play" class="quad"></div>
    <div id="fight" class="quad"></div>
    <div id="sleep" class="quad"></div>
    <div id="pet"></div>
  </div>
</body>
</html>
```
You may NOT add any other code to this file.  Any other elements that you want in the dom must use a `domStringBuilder` and `printToDom` functions to appear.

## General Requirements
Your code should be:
* Error free
* Bootstrap free
* Amazingly styled - yay SASS!!!!
* Made up of re-useable functions
* Clean

## Specific Requirements
Your website should be divided into quadrants.  Each quadrant should have a different background color and represents a different activity that you can perform.  The four activities are: eat, sleep, play, and fight.  Each of these activities should be a component with a corresponding `scss` file.  Find out more about each component below.

### Eat
The Eat component should appear in the upper left quadrant.  It should have a private variable called `full`.  This variable should be set to 100 on page load.  This module should have 2 buttons.  One should be a healthy food that adds 10 to `full` when pressed.  The other button should be an unhealthy food that subtracts 3 from `full` when pushed.

The quadrant should display the name, fullness score, and the two buttons. Each time a button is clicked the quadrant should be re-drawn to show the correct fullness score. The Full score should NEVER be larger than 100.

### Play
The Play component should appear in the upper right quadrant.  It should have a private variable called `fun`.  This variable should be set to 50 on page load.  This module should have 2 buttons.  One should be a super fun activity that adds 50 to `fun` when pressed.  The other button should be a slightly fun activity that adds 2 to `fun` when pushed.

The quadrant should display the name, fun score, and the two buttons. Each time a button is clicked the quadrant should be re-drawn to show the correct fun score. The Fun score should NEVER be larger than 100.

### Fight
The Fight component should appear in the lower left quadrant.  It should have a private variable called `strength`.  This variable should be set to 100 on page load.  This module should have 2 buttons.  One should be for running away (bravely) that adds 1 to `strength` when pressed.  The other button should be for committing violence and should subtract 10 from `strength` when pushed.

The quadrant should display the name, strength score, and the two buttons. Each time a button is clicked the quadrant should be re-drawn to show the correct strength score. The Strength score should NEVER be larger than 100.

### Sleep
The Sleep component should appear in the lower right quadrant.  It should have a private variable called `energy`.  This variable should be set to 50 on page load.  This module should have 2 buttons.  One should be for a nap and should add 50 to `energy` when pressed.  The other button should be for a deep slumber and add 60 to `sleep` when pushed.

The quadrant should display the name, energy score, and the two buttons. Each time a button is clicked the quadrant should be re-drawn to show the correct energy score.  The Energy score should NEVER be larger than 100.

## Stretch Goals
Here are some possible stretch goals. Feel free to try any that interest you or make up your own.

### Overall Progress Bar
The overall health of your Tamagochi should be based on the average of all four attributes (energy, strength, full, fun).  Use the div with the id of `progress` to display this overall score in some way.

### Pet Picture
Your pet deserves a picture.  Write a `domStringBuilder` that puts it in the div with an id of `pet`.  Make the styling look super cool.

Extra Bonus:  Let the user enter in a url for a picture on page load - make that the image that displays.

### Attribute Randomizer
Right now we have hard coded all the buttons to increase or decrease but specific amounts.  This is kinda lame.  Make all the buttons increase of decrease based on random number generators.

### Death
Something should happen when your energy, strength, full, fun, or overall heath goes to 0.  Decide what happens and make it work.

### Module Interactivity
Currently each module operates independently.  This isn't really realistic.  Modify your code so the modules interact.  Here are some sample interactions:
* When Fullness goes up energy should go down (FOOD COMA)
* When Fullness goes down strength should down
* When Strength goes down energy, full, and fun go down
* When Strength goes up energy goes up.
* When energy goes down fun goes down
