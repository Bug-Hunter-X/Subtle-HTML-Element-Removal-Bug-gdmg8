# Subtle HTML Element Removal Bug

This repository demonstrates a subtle bug related to removing HTML elements using JavaScript.  The provided code showcases the incorrect and correct methods for element removal.

## Bug Description
The primary issue lies in how the element is removed from the DOM. Using `outerHTML = ""`, while seemingly effective in removing the element visually, leaves behind a lingering reference in memory. This means that the variable referencing this element will still exist, but the element is no longer part of the DOM.