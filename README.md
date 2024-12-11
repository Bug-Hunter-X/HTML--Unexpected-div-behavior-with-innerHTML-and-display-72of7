# Uncommon HTML Bug: Unexpected Div Behavior

This repository demonstrates an uncommon bug related to manipulating a div's visibility in HTML using `innerHTML` and `style.display`.  The code attempts to initially hide a div and then show it after a delay, but due to the incorrect use of `innerHTML`, the div remains hidden.

## Bug Description
The issue stems from clearing the `innerHTML` of the div before attempting to show it.  This results in the div having no content, and even though `style.display` is changed to "block", nothing is visible.

## Solution
The solution involves removing the unnecessary `innerHTML` assignment, ensuring that the div's content persists even when temporarily hidden. 