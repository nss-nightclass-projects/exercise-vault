# Doggie Day Care
For this assignment you will be building up a doggie day care using what you know about state and props with basic React.

## Requirements
For this project we will be building out two sections of our DOM - the dogs and the employees.

### Doggies
- App should import in a DogPen component.
- App should import in a file called dogs.js that exports an array of dog objects (chose whatever key/value pairs you would like).
- App should take the array of dogs and pass it into DogPen
- DogPen should import a Dog component
- DogPen should map over the dogs array and make a Dog component
- The Dog component should display the dog in a way of your choosing.

### Employees
- App should import in a StaffRoom component.
- App should import in a file called employees.js that exports an array of employee objects (chose whatever key/value pairs you would like).
- App should take the array of employees and pass it into StaffRoom
- StaffRoom should import a Employee component
- StaffRoom should map over the employees array and make a Employee component
- The Employee component should display the employee in a way of your choosing.

### Code specification
- All your code should be error free
- If you have a `this.props.SOMETHING` in a file you should have proptypes for that thing. If the SOMETHING is an object make a shape for it