# Solar System

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

1. Create a file called planets.json and fill it with information on each of the 8 planets in our solar system.  Each planet should have the following keys:
  * name
  * imageUrl
  * description
  * isGasPlanet (true/fales)
  * numberOfMoons
  * nameOfLargestMoon
2. Create an XHR request that loads planets.json and displays them as cards with the planet name centered
![Solar System Mockup]()
3.  When the user moves their mouse over a planet card the name should dissapear and the image of the planet should take up the whole card.
4.  When the user clicks on a planet card all the cards dissapear and the only thing displayed on the page is information about the planet they clicked on.
5.  When the user clicks on the red X on a single planet that information goes away and all the original cards are displayed again.
