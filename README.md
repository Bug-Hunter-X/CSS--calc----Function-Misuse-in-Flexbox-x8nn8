# CSS `calc()` Function Misuse in Flexbox

This repository demonstrates a common error when using the `calc()` function in CSS, specifically within flexbox containers. The issue stems from the fact that `calc()`'s result depends on the context in which it's used.  If the context (the parent element) doesn't have a defined size, the calculation might be based on an undefined or unexpected value, causing layout problems.

## Bug Description:

The provided CSS uses `calc()` to determine the width of an element. However, due to the parent element's size being implicitly determined, the calculation yields incorrect results.

## Solution:

The corrected CSS explicitly sets the size of the parent container, thus enabling `calc()` to correctly determine the child element's width.