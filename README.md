# Uncommon HTML Error: Accessing DOM Element Before Load

This repository demonstrates a less common type of HTML error: attempting to manipulate a DOM element before it has been fully loaded into the browser's Document Object Model (DOM).  It also includes an example of an invalid tag placement, which is also uncommon among beginner mistakes. 

## The Problem

In the `bug.html` file, JavaScript attempts to access and modify the `innerHTML` property of the element with the ID "myDiv" before the browser has finished parsing and rendering the HTML. This leads to an error because the element does not exist yet in the DOM.

## The Solution

The `bugSolution.html` file demonstrates a corrected approach.  It uses the `DOMContentLoaded` event listener to ensure the script runs only after the entire HTML document has been parsed and the DOM is ready. It also fixes the invalid tag placement example.

This example highlights the importance of understanding the DOM's lifecycle when working with JavaScript in HTML.