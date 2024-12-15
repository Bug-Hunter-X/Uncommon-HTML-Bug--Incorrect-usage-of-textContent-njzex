# Uncommon HTML Bug: Incorrect usage of textContent

This repository demonstrates a subtle bug related to updating the content of a div element in HTML. The bug showcases the difference between using `textContent` and `innerHTML` for modifying the content of an HTML element.  Incorrect usage of `textContent` can lead to unexpected behavior or potential security vulnerabilities.

## Bug Description

The `bug.html` file contains a div element whose content is updated using `textContent`. This approach can unexpectedly strip out HTML markup when it should preserve the structure. The `bugSolution.html` file shows the correct and safe way to handle this scenario.

## Bug Solution

The solution is to use `innerHTML` when dealing with HTML content to maintain its structure. `textContent` should be used when the div or any similar element is only to contain plain text without markup tags to avoid potential XSS vulnerabilities.