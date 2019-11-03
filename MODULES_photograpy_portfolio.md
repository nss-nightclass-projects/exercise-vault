# Photography Portfolio
## Introduction
You are creating a photography filtering site for a famous photographer who wants to showcase their work.

## Planning Requirements
* Create a new github repo called `photography-portfolio`
* Create a github project on this repo
* Create feature tickets for this assignment
* Create wireframes for this project and attach them to the appropriate project.
* Be VERY careful about your data structure on this project.  You should probably have an instructor review it before you start.

## Technical Requirements
* You must use [Boostrap 4](https://getbootstrap.com/docs/4.0/getting-started/introduction/) to style your page components.
* Your JS file should be comprised of functions, no actions should happen in your code outside of a function
* Your HTML and JS should all have proper indentations
* You should be using [webpack](https://github.com/nss-nightclass-projects/Night-Class-Resources/blob/master/book-2-patterns-and-tools/chapters/task-runners.md) to compile your JS and SCSS
* You should be writing all your CSS/SCSS in SCSS files
* Your JS code should be eslint error and warning free
* For this project ALL your photographs should be image urls - DO NOT store the photos locally.

## User stories
* As a user, when the page loads, I should see all my photographs.
* As a user, when the page loads, I should see a dropdown to filter my photographs by direction (portrait, lanscape, selfie)
* As a user, when the page loads, I should see a dropdown to filter my photographs by filter (black and white, color, sepia)
* As a user, when the page loads, I should see a dropdown to filter my photographs by occasion (wedding, graduation, travel, family)
* As a user, when the page loads, I should see a dropdown to filter my photographs by location (pick at least 5 location)
* As a user, when I select an option in a dropdown I should only see images that fall in that category.
* As a user, I would like clear all button, that is disabled if no filters are selected.
* As a user, I would like clear all button, that when clicked shows all photographs again.

**FOR MVP** - your filters can work one at a time - ie each time a dropdown is changed that is the only one that applies.

## Bonus
Multiple filters - If I select multiple dropdowns I should only see photos that meet all my selections.  For example if I select weddings, black and white, and Japan I should only see photos of weddings in Japan that are black and white.