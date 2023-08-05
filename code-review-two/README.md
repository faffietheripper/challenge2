# Code Review Questionnaire #2 [20mins]

The "Shopping Cart" Lab

- Review the [Lab Instructions](./instructions.md)
- Review the [student's submission](./src)
  - (Optionally) Launch a dev server to run the code within `./src` by running `npm run start`
- Given the following problem statements from the student, what would you say to advise them?
  - "When I add items to my cart, everything works. Then if I goto the cart page the cart is empty"
  - This was happenning because the student was using different local storage keys to save data and retrieve the data.
 

- Have best practices been followed?
- Mostly yes however the student should try to assign values using const instead of let because it clearlky shoiws that the valkue can not be changed or reasigned and the advantage of doing this is that const variables can not be redeclared within the same scope with prevents confusion on bigger projects.


- What would you recommend they do to extend this?
- The student can add alert messages to see when a product has been successfuly saved to the cart so that they dont see the error at the end if it happens again.
- The stident can add a function that chexks if there is products in the local storage and load them back onto the cart storage when you run the code.


- Are you able to identify any issues with the codebase?
- The name of the array with cart instances on line 14 was this.items however the student was trying to set the instances to this.item
