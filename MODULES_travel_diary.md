# Travel Diary
## Introduction
Traveling is fun but it can sometimes be hard to remember what happened on a trip.  For this project you will be creating a travel diary to keep track of your adventures

## Planning Requirements
* Create a new github repo called `travel-diary`
* Create a github project on this repo
* Create feature tickets for this assignment
* Create wireframes for this project and attach them to the appropriate project.

## Technical Requirements
* You must use [Boostrap 4](https://getbootstrap.com/docs/4.0/getting-started/introduction/) to style your page components.
* Your JS file should be comprised of functions, no actions should happen in your code outside of a function
* Your HTML and JS should all have proper indentations
* You should be using [webpack](https://github.com/nss-nightclass-projects/Night-Class-Resources/blob/master/book-2-patterns-and-tools/chapters/task-runners.md) to compile your JS and SCSS
* You should be writing all your CSS/SCSS in SCSS files
* Your JS code should be eslint error and warning free

## Requirements
1. Create an array of objects that represent places you've been or want to go. These objects should have a title, image and description. You need at least 5 unique objects in the array.
1. Print each of the objects to the DOM in a "card" that also has it's own input box and submit button. There should be 3 "cards" per row.
1. The final result of printing the array should look like the following mockup:
![Travel Diary Mock Up Part 1](https://github.com/nss-nightclass-projects/exercise-vault/blob/master/images/TravelDiaryPt1.png?raw=true)
4. The user should be able to type in the text box for a specific location, click the submit button on that card, and their entry should appear in a "diary" below the cards.
	- The diary entry should contain the name of the location from the card the user was typing in (and hit the submit button in). It should also contain only the text that was in the text box from that card.
	- The text box for that card should be cleared upon submission.
5. The diary entries should build up as the user continues to type in cards and submit their entries. Newest entries should appear at the bottom. The final result will look like the following mockup:
![Travel Diary Mock Up Part 2](https://github.com/nss-nightclass-projects/exercise-vault/blob/master/images/TravelDiaryPt2.png?raw=true)


## Bonus
* Once a user has written about a place at least once, change the color of the card for that place.
* Create a form so a user can add new locations.
* Add a timestamp to the diary entries.
* Users should be able to delete diary entries.
* Users should be able to edit their diary entries.
