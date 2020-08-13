# Cat Cafe

You've been tasked with making a tracking app for Cat Cafes. Each cafe has a number of cats that belong to them, and only them. These cafes are jelous: NO SHARING!!!

## Requirements

ERD:

### Cafe
field | type
----|----
id | string
name | string
location | string
isOpen | bool
uid | string

### Cat
field | type
----|----
id | string
name | string
breed | string
imgUrl | string
cafeId | string
isNice | bool

## User Stories

### Authentication
* As a user, who is logged out, I should only be able to see the authentication screen
* As a user who is logged out, I would like to be able to authenticate by clicking on a button.
* As a user who is logged out, I would like to be able to click on an authentication button and login via google.
* As a user who is logged in, I should not be able to see the authentication button.
* As a user who is logged in, I should be able to see the CafeContainer component.

### CREATE Cafes
* As an authenticated user, I should be able to click a button that displays a form to add a new cafe that I own.
* As an authenticated user, when I fill out the form and submit a new Cafe should be created in firebase and should now show in my CafeContainer component.

### READ Cafes
* As an authenticated user, I should be able to see the CafeContainer component with all the cafes I have created.
  * The CafeContainer should be a `<table>` element
* As an authenticated user I should not be able to see cafes that were created/are owned by another user.

### UPDATE Cafes
* As an authenticated user, I should be able to see an edit button on each cafe card.
* As an authenticated user, when I click the edit button I should see a form with the cafe information for that cafe pre-populated.
* As an authenticated user, I should be able to edit the information in the form and hit the submit button.
* As an authenticated user, when I submit the edit form firebase should be updated (PUT request) and the CafeContainer component should update

### CREATE Cats
* When viewing a single Cafe:
  * As an authenticated user, I should be able to click a button that displays a form to add a new Cat that the current cafe owns.
  * As an authenticated user, when I fill out the form and submit a new Cat should be created in firebase and should now show in the Cafe component.

### READ Cats
* When viewing a single Cafe:
  * As an authenticated user, I should be able to see the Cafe component with all the Cats I have created.
  * As an authenticated user I should not be able to see cats that were are owned by another Cafe.

### DELETE Cats
* When viewing a single Cafe:
  * As an authenticated user, I should be able to delete a Cat from a Cafe component

### UPDATE Cats
* When viewing a single Cafe:
  * As an authenticated user, I should be able to see a edit button on each cat card.
  * As an authenticated user, when I click the edit button I should see a form with the cat information for that cat pre-populated.
  * As an authenticated user, I should be able to edit the information in the form and hit the submit button.
  * As an authenticated user, when I submit the edit form firebase should be updated (PUT request) and the Cafe component should update


## BONUS

### Trade Cats
* As an authenticated user I should be able to move a Cat from one Cafe to another
  * When viewing a Cafe there should be a "move" button, which displays a list of Cafes this cat can be moved to. The UI/UX is up to you
