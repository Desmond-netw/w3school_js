JavaScript events are actions or occurrences that happen in the web browser, which can be detected and responded to using JavaScript. Events are the foundation for making web pages interactive. Here are some commonly used events in JavaScript, including onchange and onclick:

# ** Common JavaScript Events **

### onclick

Triggered when an element is clicked.
Often used on buttons, links, and other clickable elements.
Example:
html
Copy code
<button onclick="alert('Button Clicked!')">Click me</button>
onchange:

Triggered when the value of an element changes, typically for input fields like <input>, <select>, or <textarea>.
Useful for validating user input or updating UI based on the input.
Example:
html
Copy code
<input type="text" onchange="alert('Input changed!')" />
onmouseover:

Triggered when the mouse pointer moves over an element.
Commonly used for hover effects.
Example:
html
Copy code
<div onmouseover="this.style.backgroundColor='yellow'">Hover over me!</div>
onmouseout:

Triggered when the mouse pointer moves out of an element.
Example:
html
Copy code
<div onmouseout="this.style.backgroundColor='white'">Move mouse out!</div>

### onkeydown:

Triggered when a key is pressed down on the keyboard.
Often used for handling keyboard shortcuts or text input.
Example:
html
 - Copy code
    -<input type="text" onkeydown="alert('Key pressed!')" />

### onkeyup:

Triggered when a key is released after being pressed.
Can be used to capture input after the user finishes typing.
- Example:
    html
    Copy code
  - <input type="text" onkeyup="alert('Key released!')" />
onfocus:

Triggered when an element (like an input field) gains focus.
Example:
html
Copy code

<input type="text" onfocus="this.style.backgroundColor='lightblue'" />
onblur:

Triggered when an element loses focus.
Example:
html
Copy code
<input type="text" onblur="this.style.backgroundColor='white'" />
onsubmit:

Triggered when a form is submitted.
Often used for form validation before submission.
Example:
html
Copy code
<form onsubmit="alert('Form submitted!')">
  <input type="submit" value="Submit" />
</form>
onload:

Triggered when the page or an image is fully loaded.
Commonly used for initializing functions when the web page loads.
Example:
html
Copy code
<body onload="alert('Page loaded!')">
oninput:

Triggered when an element receives input from the user. Unlike onchange, it is fired as soon as the input value is modified.
Example:
html
Copy code
<input type="text" oninput="console.log(this.value)" />
onresize:

Triggered when the window is resized.
Example:
html
Copy code
<body onresize="alert('Window resized!')">
ondblclick:

Triggered when an element is double-clicked.
Example:
html
Copy code
<button ondblclick="alert('Double clicked!')">Double Click Me</button>
onscroll:

Triggered when the user scrolls an element with a scrollbar (like a <div> or the browser window itself).
Example:
html
Copy code
<div style="overflow-y: scroll; height: 100px;" onscroll="alert('Scrolling!')">
  Scrollable content here...
</div>
onerror:

Triggered when an error occurs while loading an external resource like an image or script.
Example:
html
Copy code
<img src="invalid.jpg" onerror="alert('Error loading image!')" />
How Events Are Used:
Inline Event Handlers: As shown in the examples above, events can be directly added in HTML using inline attributes.
JavaScript Event Listeners: Modern best practice is to attach events using JavaScript with addEventListener() to keep HTML and JavaScript separate. Example:
javascript
Copy code
document.querySelector('button').addEventListener('click', function() {
  alert('Button clicked using addEventListener!');
});

## Summary:

JavaScript events like onclick, onchange, onmouseover, etc., allow interaction with web elements by reacting to user actions such as clicks, key presses, input changes, and more. These events can be used to create dynamic and interactive user experiences on a webpage.