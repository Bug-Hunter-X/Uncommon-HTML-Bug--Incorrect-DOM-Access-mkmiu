# Uncommon HTML Bug: Incorrect DOM Access

This repository demonstrates a subtle bug that can occur in HTML when working with the DOM (Document Object Model).  The bug arises from a typo in accessing the DOM element, leading to an unexpected runtime error. While seemingly minor, typos like this can be challenging to detect.

## Bug Description

The bug lies in the JavaScript code within the HTML file.  It attempts to use `document.getElementByIdx('myDiv')` to access an element with the ID 'myDiv'. Notice that there's an extra 'x' in `getElementByIdx`. This incorrect function call will throw an error because `getElementByIdx` does not exist.

## Solution

The solution is simple: correct the typo in the function call. Use `document.getElementById('myDiv')` to properly access the element.
