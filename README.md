# Require Test
This is a test to see if the order files are listed in a require block effects the order they're loaded in the browser.

Good require modules should not need to be loaded in any particular order, but in the edge case that they do knowing this would help.

## Setup
Run `npm install` to install dependencies.
Run `node server` to run page on [localhost:3000](http://localhost:3000/)

## Hypothesis
In the console run `getFiles()` files.  `short-file` should come first.
Refresh and run `getFiles(1)`.  This time `long-file` should come first.

## Conclusion
The order listed in the require block does NOT effect the order its loaded on the page.  Items are loaded as they are ready.
