# Almost Amazon

## Instructions
You will be building a modular version of the greatest book store known to humankind - Almost Amazon.  This bookstore has a single book (of your choosing) and some awesome realated styling (if you would like).  

At minimum your Almost Amazon site should have:
1. A store with a single book
1. The ability to put the book in your cart

## Tech Requirements
This assignment is extremely simple - whats important here is to understand the new way we are organizing our files.  You should have the following files:

```
- javascripts/
  - main.js # the entry point to your app
  - components/
    - store.js # should hold your book object as a private variable.  Should have an event listener for the add to cart button
    - cart.js # should use a get method on the store module to get the price of the book. Should call the printToDom function and display the cart.
  - helpers/
    - util.js # should have the printToDom function.
- index.html # usual stuff with all the html and script tags
- main.css # for styling.  At minimum you should use the bootstrap grid system but feel free to style however you would like.
```

## Planning Requrements
* Create a github project for this assignment.
* You should make cards/tickets based on deliverable features, i.e. print the store with the single book the page, create add to cart button which triggers a console log in cart.js, print cart to dom on button click.

## Bonus
- Create a discount button that will discount the price of the book by some percentage. The logic for this should exist in either your util.js file or within a new module inside the `helpers/` directory. The discount should only apply once to the item (meaning, I shouldn't be able to continually click the button and have the price decrease).
