# Dinosaur Kennel
## Introduction
Welcome to Jurassic Kennel - where people board their dinosaurs for the day!  You have been tasked with creating a dashboard for the Kennel owners to know the status of each dinosaur in their care for the day.

## Planning Requirements
* Create a new github repo called `dinosaur-kennel`
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

## User stories
* As a kennel owner, if a new dinosaur is dropped off I need a way to add a new dinosaur to my UI.
* As a kennel owner, I would like to keep track of the dinosaurs name, age, color, type, location, image, and health score.
* As an application, when a new dinosaur is added, I am going to randomly give them a health score between 0 and 100.
* As a kennel owner, I want a way to visually see where a dinosaur is inside my facility (main kennel, hospital, or graveyard)
* As a kennel owner, I should have buttons for each dinosaur to feed them or send them on an adventure.
* As a kennel owner, if I feed a dinosaur their health should increase by a random amount between 0 and 100 but never go over 100.
* As a kennel owner, if I send a dinosaur  on an adventure their health should decrease by a random amount between 0 and 100.
* As an application, if the health of a dinosaur goes below 40 their location should change to the hospital
* As an application, if the health of a dinosaur goes to 0, the dinosaurs location should change to the graveyard, all buttons on them should be disabled, and a skull and crossbones should appear over their picture.
* As a kennel owner, if a person comes to pick up their dinosaur I should be able to delete them from my kennel (dead dinosaurs should never be deleted).
