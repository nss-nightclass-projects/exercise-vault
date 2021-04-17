# Shark Attack
Oh no your entire class has fallen into a pool infested with sharks and they are HUNGRY.

## Requirements
The focus of this assignment is state and props in react.
* You will NOT be using firebase.
* Every file that has a `this.props` should have the appropriate proptypes defined.
* DO NOT COPY PASTE ANYTHING - hand type every part of this assignment copy/paste doesn't teach you to read errors.

### React Components
In addition to the `App` component your application should have the following components:
* `SharkTank` - the pool that all living students are swimming in
* `LiveStudent` - a card of your choosing that gets called from the SharkTank component inside a map.
* `Graveyard` - the burial ground for students who have not made it...
* `GraveStone` - a card of your choosing that gets called from the Graveyard component inside a map.


### Setting up the students
* Create a `src/helpers/data/studentsData.js`
  *  This file should have an array at the top called `students`
  * The array should have one student object for every student in the class (if you don't remember the other students in your class thats SUPER awkward but everyone is listed in codetracker so go there and figure it out)
  * Each student object should have the following keys: id, firstName, lastName, isDead
  * The `isDead` key should be set to `false` for everyone on load
  * This file should export a function called `livingStudents` that returns an array of the students where `student.isDead === false`
  * This file should export a function called `dearlyBeloved` that returns an array of the students where `student.isDead === true`
  * This file should export a function called `followTheLight` that takes in an id, finds that student, and changes `student.isDead` to `true`
* The `App.js` file should call the two functions exported out of `studentsData.js` and pass the arrays into the appropriate components (`dearlyBeloved` passes into `<Graveyard />` and `livingStudents` passes into `<SharkTank />`).

### Live Student User Stories
* As a user, when the page loads, I should see a nice big shark tank.
* As a user, when the page loads, I should see all live students represented in the shark tank.  You can do this however you want - bootstrap card or something more exciting (animated lil fishies?!?!?!?)
* As a user, when the page loads, I should see a dangerous looking button in the shark tank that says SHARK ATTACK.
* As a user, when I click on the SHARK ATTACK button, the app should pick a random live student and change their `isDead` key to `true`.

### Graveyard User Stories
* As a user, when a student dies/is dead they should no longer be displayed in the shark tank.
* As a user, I should be able to see all dead students in the graveyard - you can display them however you want (bootstrap cards a minimum but gravestones would be way cooler and appropriately morbid)
