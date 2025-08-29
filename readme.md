1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

Ans:

getElementById("id"): Selects a single element by its ID. Returns one element.

getElementsByClassName("class"): Selects all elements with a given class. Returns an HTMLCollection (live).

querySelector("selector"): Selects the first element that matches a CSS selector.

querySelectorAll("selector"): Selects all elements that match a CSS selector. Returns a NodeList (static).

2. How do you create and insert a new element into the DOM?

Ans:
Steps to create and insert a new element:

1. Use document.createElement("tag") to create a new element.

2. Set its content using element.textContent or element.innerHTML.

3. Insert it into the DOM using parent.appendChild(element) or parent.insertBefore(newElement, referenceNode).

Example:

const li = document.createElement('li');
li.textContent = "New Item";
document.getElementById('list').appendChild(li);

3. What is Event Bubbling and how does it work?

Ans:
Event Bubbling is a DOM event mechanism where an event starts at the target element and then bubbles up through its parent elements all the way to the root.

This is default behavior and helps handle events efficiently on parent elements.

4. What is Event Delegation in JavaScript? Why is it useful?

Ans:
Event Delegation is a technique where a single event listener is added to a parent element to handle events for its child elements.

Why it is useful:

Works even if new child elements are added dynamically.

Reduces code duplication and saves memory.

5. What is the difference between preventDefault() and stopPropagation() methods?

Ans:

preventDefault(): Prevents the default browser action (e.g., navigating to a link).

stopPropagation(): Stops the event from bubbling or capturing to parent elements.
