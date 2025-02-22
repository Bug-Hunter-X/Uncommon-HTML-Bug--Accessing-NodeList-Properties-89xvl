# Uncommon HTML Bug: Accessing NodeList Properties

This repository demonstrates an uncommon bug in HTML related to accessing properties of a NodeList.
The bug occurs when attempting to directly access a non-existent property of a NodeList returned by `document.querySelectorAll`. NodeLists do not have custom properties; they're collections of nodes.

## Bug Description
Attempting to access a non-existent property of a NodeList will result in a `TypeError`. The correct approach is to access individual nodes within the NodeList using array indexing (e.g., `nodeList[0]`).

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Observe the error in the browser's console.