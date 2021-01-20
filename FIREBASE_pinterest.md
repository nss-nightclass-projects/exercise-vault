# Pinterest

Your team has been tasked with creating pinterest.  If you live under a rock and have never used pinterest before go figure out what it does. TLDR; users create boards and can pin urls to the boards

## Requirements
* Clean code - single responsibility principle
* ES6 Modules bundled with webpack
* No errors - linters should be clean
* Jquery for any DOM manipulation (selectors, modifying css classes, events)
* SASS and Bootstrap for styling
* Completely planned out - before each section you should be making new cards before you code.  You should have wireframes and an ERD

## HW Parts

### Part 1: ERDs and Authentication
* Create an ERD for pinterest (do this in studygroup)
* Create a new githup repo called pinterest
* Create a setup branch and setup webpack (make a ticket for this first)
* Create a new firebase project and enable google authentication
* Create an authentication branch and add in all authentication that we did in class (navbar with logout button, google login button)
* When your user is logged out they should see the navbar with only a brand.  And an h1 on the page that says PINTERST (make a `home` component for this)
* When your user is logged in they should see a navbar with a brand and a logout button and an H1 on the page that says Boards (make a `boards` component for this)

### Part 2: READ
#### Setup
* Create some json data
* Import that data into firebase

#### User Stories
* As a user, when I am logged in and the page loads, I should see all the boards that belong to me.

* As a user, when I click on one of my boards, I should see a single board view that shows all pins for that board.

* As a user, when I am on the single board view, there should be some way to go back to all my boards.

### Part 3: DELETE
* As a user, I should be able to delete a pin from one of my boards.

* As a user, I should be able to delete one of my boards.

* As a user, when I delete one of my boards all pins that were on that board should be deleted as well.

### Part 4: CREATE
* As a user, I should be able to create a new pin.

* As a user, I should be able to create a new board.

### Part 5: UPDATE
* As a user, I should be able to change which board a pin belongs to.

### Part 6: Deploy and Readme
* As a user I should be able to use your app on the internet - it should be [deployed using firebase or Netlify](https://github.com/nss-nightclass-projects/Night-Class-Resources/blob/master/book-3-data-driven-applications/chapters/firebase-deploy.md).

* As a developer, I want to see an amazing README for this project.
