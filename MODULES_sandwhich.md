# Sandwich Maker

## Requirements

Create a sandwich order form that allows the user to select all the ingredients for a custom deli sandwich. Each of the following should be separate modules:

+ bread
+ meat
+ cheese
+ condiments
+ veggies
+ sandwhich

Your project should have one HTML file that has:

+ A section of options for each sandwich part 
+ The ability to select multiple, or zero, choices for each section (such as turkey _and_ bacon, or "no meat") 
+ An empty DOM element into which the final sandwich order and its cost will be inserted  

The ingredient choices should be stored as JS objects that contain the 3 key value pairs: id, name, and price(in cents). 
```
{id: "meat1", name: "turkey", price: 90}
```

Make sure the ingredient objects cannot be accessed by the other modules except through an accessor (getter) method.  

Each of your modules should be completely self contained.

> Don't worry about exposing the prices to the user until you display the final cost. This is just an exercise, not a business model.
