# Travel Diary

## Setup
1. Create a new repository on GitHub
1. Connect the repository with a directory in single-page-apps/exercises
1. Create a GitHub project and thoroughly plan out the project, breaking it into well-documented tickets.
1. After pushing your base README.md to master, you should be working off branches
1. Create an index.html, main.js and main.css and link them all together.

## Technical Requirements

1. Single responsibility prinicple: Each function should be responsible for one thing.
1. No frameworks or libraries (Bootstrap/Materialize, jQuery, etc); everything is vanilla

## Requirements

1. Create an array of objects that represent places you've been or want to go. These objects should have a title, image and description. You need at least 5 unique objects in the array.
1. Print each of the objects to the DOM in a "card" that also has it's own input box and submit button. There should be 3 "cards" per row.
1. The final result of printing the array should look like the following mockup:
![Travel Diary Mock Up Part 1](https://github.com/nss-nightclass-projects/exercise-vault/blob/master/TravelDiaryPt1.png?raw=true)
4. The user should be able to type in the text box for a specific location, click the submit button on that card, and their entry should appear in a "diary" below the cards.
	- The diary entry should contain the name of the location from the card the user was typing in (and hit the submit button in). It should also contain only the text that was in the text box from that card.
	- The text box for that card should be cleared upon submission.
5. The diary entries should build up as the user continues to type in cards and submit their entries. Newest entries should appear at the bottom. The final result will look like the following mockup:
![Travel Diary Mock Up Part 2](https://github.com/nss-nightclass-projects/exercise-vault/blob/master/TravelDiaryPt2.png?raw=true)

BONUS ALERT: Once a user has written about a place at least once, change the color of the card for that place.

BONUS BONUS ALERT: Add a timestamp to the diary entries.

BONUS BONUS BONUS ALERT: Users should be able to delete diary entries.

![But wait there's more...](http://s2.quickmeme.com/img/a7/a78ae76da19c1a0f9e0e9b2f7e6229e70bd36cf7bc5b2f29b5f8900face50234.jpg)

BONUS BONUS BONUS BONUS ALERT: Users should be able to edit their diary entries.
