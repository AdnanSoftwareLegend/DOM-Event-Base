

1. Difference between getElementById, getElementsByClassName, querySelector, querySelectorAll

getElementById("id")
  * Selects ONE element by id.
  * Returns a single element object or null.
 getElementsByClassName("class")
  * Selects ALL elements with a class name.
  * Returns a live HTMLCollection.

 querySelector("css-selector")
  * Selects the FIRST element that matches a CSS selector.
  * Returns a single element object.

 querySelectorAll("css-selector")
  * Selects ALL elements that match a CSS selector.
  * Returns a static NodeList.



2. How to Create and Insert a New Element into the DOM

let newDiv = document.createElement("div");
newDiv.textContent = "Hello World!";
document.body.appendChild(newDiv);


3. What is Event Bubbling and How Does It Work?

Event bubbling means an event starts from the target element and moves upward to parent elements.
Example:
Child clicked -> Parent clicked



4. What is Event Delegation in JavaScript? Why is it useful?

 Attaching one event listener to a parent instead of many listeners to children.
 Uses bubbling to handle events from child elements.
Useful because:
  * Better performance
  * Works for dynamically added elements
  * Cleaner code



5. Difference between preventDefault() and stopPropagation()

preventDefault():
  * Stops the browser's default behavior (e.g., prevent form submit).

stopPropagation():
  * Stops the event from bubbling up (or capturing down).

