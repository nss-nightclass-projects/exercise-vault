# Mushroom Picker
Now that we are in the apocalypse and super HUNGRY its time to go mushroom picking.  Just like little red riding hood you have been given a basket and sent into the woods.  While you are in the woods you are going to pick some mushrooms.  Ideally you catch them ALL - but not the poisonous or deadly ones.

## Requirements
The focus of this assignment is state and props in react.
* You will NOT be using firebase.
* Every file that has a `this.props` should have the appropriate proptypes defined.
* DO NOT COPY PASTE ANYTHING - hand type every part of this assignment; copy/paste doesn't teach you to read errors.
* You can style this in any way you want - at minimum use bootstrap to make it clean

### React Components
In addition to the `App` component your application should have the following components:
* `Forest` - where all the mushrooms grow
* `Basket` - the mushrooms you have picked
* `Mushroom` - some type of SINGLE mushroom card - this component will get called inside map functions in both Forest and basket

### Setting up the mushrooms
* Create a `src/helpers/data/mushroomData.js`
  * This file should have 2 arrays at the top - one called `mushrooms` and the other called `basket`
  * Each mushroom object should have the following keys: id, name, description, imgUrl, isMagic, isPoisonous, isDeadly
  * Your seed data should have 20 mushrooms:
    * 1 magic mushroom (isMagic=true)
    * 3 poisonous mushrooms (isPoisonous=true)
    * 1 deadly mushroom (isDeadly=true)
    * 15 regular mushrooms (isMagic=false, isPoisonous=false, isDeadly=false)
  * This file should export a function called `getMushrooms` that returns an array of ALL the mushrooms
  * This file should export a function called `getBasket` that returns an array of ALL the basket items
  * This file should export a function called `pickAMushroom` that picks a random mushroom from the array and adds it to the `basket` array
  * Add any additional helper functions to this file that you think you need
* The `App.js` file should call the `getMushrooms` and `getBasket` and pass the arrays into the appropriate components (array of mushrooms goes to the `Forest` and basket array goes into `Basket` component).

### User Stories
* As a user, when the page loads, I should see all the mushrooms in the forest.
* As a user, when the page loads, I should see my empty basket.
* As a user, when the page loads, I should see a button thats says "Pick Mushroom"
* As a user, when I click the "Pick Mushroom" button, a random mushroom should be placed in my basket.
* As a user, I should be able to have more than one of the same mushroom in my basket.  Stretch Goal: only display one mushroom but state the # of that type of mushrooms you have
* As a user, if I pick a poisonous mushroom (isPoisonous === true) two other mushrooms in my basket should DIE - ie get removed (in addition the poisonous mushroom picked should NOT show up in the basket)
* As a user, if I pick a deadly mushroom (isDeadly === true) ALL the mushrooms in my basket should DIE - ie get removed (in addition the poisonous mushroom picked should NOT show up in the basket)
* As a user, if I pick a magic mushroom (isMagic === true) then I should get one of each of the non magic, non poisonous, and non deadly mushrooms added to my basket and I should WIN (in addition the magic mushroom picked should NOT show up in the basket)
* As a user, if my basket has one (or more) of each type of mushroom that is non poisonous, non deadly, or non magic (ie regular plain mushroom) then I have collected them all and I should WIN.
* As a user, if I WIN, something cool should happen.
* As a user, if I pick a poisonous or deadly mushroom, something dark and scarry should happen
