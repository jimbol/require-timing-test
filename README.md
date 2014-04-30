## Require Test
This is a test to see if the order files are listed in a require block effects the order they're loaded in the browser.</p>

# Hypothesis
In the console run `getFiles()` files.  `short-file` should come first.</p>
Refresh and run `getFiles(1)`.  This time `long-file` should come first.</p>

# Conclusion
The order listed in the require block does NOT effect the order its loaded on the page.  Items are loaded as they are ready.</p>
