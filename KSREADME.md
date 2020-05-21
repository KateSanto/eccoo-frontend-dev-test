# Enhancements
## CSS / Page layout
* I've added a page header and a form header to help user understand what the site is and what the form is for.
* I've removed data output from the frontend form as it's not usable for the user (and it wasn't in the layout given in the task). There might be a user story that justifies the input being presented back to the user. In that case, a dev will need to recover that bit of code for manipulation and/or safe storage of the inputted data, so instead of completely removing the code, I've simply commented it out, with a note explaining why.

## Accessibility
* I've used [axe](https://www.deque.com/axe/) to look for accessibility issues. The report generated displayed no errors.
* I struggled to style the radio buttons beyond making them bigger. In the proposed layout we had to follow, they are black and white, but in my frontend you'll notice they are grey instead. I spent a bit of time researching to figure out how to make custom radio buttons and, because it was taking too long, I decided that, unless the colours posed an accessibility issue, I wasn't going to style them further. There were no accessibility/contrast issues, so... grey radio buttons it is.

## Codebase
* I've imported Bootstrap and Google Fonts into the project for user-friendly features and an easy-to-read typeface.
* I've created a new macro for the radio buttons. Since this is a short form, it might have been ok to define each radio button individually, but using a macro had two advantages:
  * It kept the new code consistent with the existing code
  * It's easier to scale. If a dev needs to add more fields in a future iteration of the page, they would only need to type in a few characters instead of a full block of code for each new field.