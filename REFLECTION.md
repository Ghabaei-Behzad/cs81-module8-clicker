// Behzad Ghabaei
// CS 81 - JavaScript
// Assignment 8A - spaceClicker.html
// Reflection.md
// Instructor Seno
// 1/29/2026
# Cookie Clicker Reflection

## What helped you understand DOM interaction best?
The most helpful part was seeing the examples of how buttons work (first, a button is created in the HTML mark-up, then adjustments
can be made inside the JavaScript <script> tags.) The immediate connection between the document.getElementById "handle" and the actual text on the screen, shows me how to apply the code to the web page.  When realizing that textContent acts like a bridge between my
JavaScript logic and the user’s eyes, the concept of the Document Object Model became much more solid. This turned the webpage from a static
document into a dynamic object which I could control and style. I looked at several resources such as the MDN Web Docs on DOM.  I also looked at how scripts
interact with HTML through videos and crash courses on you tube.

## How did you choose your milestone messages?
The milestones I chose were at 10, 25, 50, and 100 clicks.  I chose messages for the user to read as they clicked. Each milestone has a
different button emoji and background color too.  I chose a dark color for the background at 0 clicks, and an idea I had was to adjust the
background color by changing the last digit of the hex#.  More colors can be found at www.colorhexa.com.
At 10 clicks I could see that the code was working.  I ended the milestones at 100 with purple as the background color. The goal was to
match the visual theme of a "Supernova" while rewarding the player’s effort with increasing descriptions. I decided to change the button emoji and background color at each milestone of 10, 25, 50, and 100.  There was not a large variety of space theme emojis which were categorized as earth and sky.

## What challenge or bug surprised you?
I was surprised by how important it is to keep the variable count outside the event listener function. Initially, if I had reset it to 0
inside the function, the counter would never have gone past 1 because it would restart on every click. This taught me about variable scope
and how data needs to be in the right place to be remembered across multiple events. W3Schools helped me with the "try it editor" and examples.
A surprise I encountered is that I could not use an emoji to rotate around the screen, but an image would have worked using an HTML <img> tag. I researched a way to do this by using <span> with relative positioning for emojis.  This does work and is from Chapter 14: DOM. Here is the code:
1.) <p> I used: style ="text-align: center; font-size: 50px;"
    <span> I used: id="moving-emoji" style="position: relative">🍪</span></p>
2.)  let emoji = document.querySelector("#moving-emoji");
3.)  let angle = Math.PI / 2;
4.)  function animate(time, lastTime) {
     if (lastTime != null) { angle += (time - lastTime) * 0.002; }
     emoji.style.top = (Math.sin(angle) * 40) + "px";
     emoji.style.left = (Math.cos(angle) * 100) + "px";
5.)  requestAnimationFrame(newTime => animate(newTime, time)); }
     requestAnimationFrame(animate);
This additional feature could make this app much more entertaining.

## What personal twist did you add?
Instead of a bakery theme, I added a "Galactic Supernova" twist that changes the entire environment, as you click the mouse. Collecting the emojis at emojipedia.org was helpful.  I used JavaScript to modify the document.body.style.backgroundColor and even change the button's emoji from a star to a galaxy at 100 clicks ( the final milestone.) This made it look and feel less like a simple counter and more like a progressing "story" or game. 
## What real-world app uses this kind of interaction?
Social media platforms like Instagram use this exact addEventListener logic for their "Like" buttons. Clicking the heart triggers an event that updates a counter and changes the heart's color. Shopping apps like Amazon also use it for "Add to Cart" buttons to update the total without reloading the page. Even progress bars in fitness apps rely on these event-driven updates to show you your status.  Major companies like Facebook and Netflix use addEventListener. In conclusion, I would like to see more examples on event handling to improve my knowledge of app development. (getting information from PravaahConsulting.com)

