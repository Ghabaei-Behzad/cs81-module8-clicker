// Behzad Ghabaei
// CS 81 - JavaScript
// Assignment 8A - spaceClicker.html
// Reflection.md
// Instructor Seno
// 1/29/2026
# Cookie Clicker Reflection

## What helped you understand DOM interaction best?
The most helpful part was seeing the examples of how buttons work ( first a button is created in the HTML mark-up, then adjustments
can be made inside the JavaScript <script> tags. The immediate connection between the document.getElementById "handle" and the actual
text on the screen, shows me how to apply the code to the web page.  When realizing that textContent acts like a bridge between my
JavaScript logic and the user’s eyes, the concept of the Document Object Model much more solid. This turned the webpage from a static
document into a dynamic object which I could control and style. I looked at several resources such as the MDN Web Docs on DOM and scripts
interact with HTML. Also, videos and crash course you tube examples.

## How did you choose your milestone messages?
The milestones I chose were at 10, 25, 50, and 100 clicks.  I chose messages for the user to read as they clicked. Each milestone has a
different button emoji and background color too.  I chose a dark color for the background at 0 clicks, an idea I had was to adjust the
background color by changing the last digit of the hex#.  More colors can be found at www.colorhexa.com.
At 10 clicks I could see that the code was working.  I ended the milestones at 100 with purple as the background color. The goal was to
match the visual theme of a "Supernova" while rewarding the player’s effort with increasing descriptions. 

## What challenge or bug surprised you?
I was surprised by how important it is to keep the variable count outside the event listener function. Initially, if I had reset it to 0
inside the function, the counter would never have gone past 1 because it would restart on every click. This taught me about variable scope
and how data needs to be in the right place to be remembered across multiple events. W3Schools helped me with the "try it editor" and examples.
A surprise I encountered is that I could not use an emoji to rotate around the screen, but an image would have worked. with an HTML img tag. 
## What personal twist did you add?

## What real-world app uses this kind of interaction?
