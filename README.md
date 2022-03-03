This repo contains fixes for the Big O lecture slides and lab solutions.

`original-index.js` contains the lab problems and their original solutions. `index-revised.js` includes the same problems, with corrected solutions and explanations. 

The `slide-correction` folder contains an incorrect example that many of the original lab solutions were based on. The `slide-correction.md` file contains an explanation of the mistake in the slide, as well as an accurate example of a function with linear space complexity.


# A short guide to calculating space complexity

In JS, three things make space complexity increase:
- Assigning variables
- Creating new data structures (arrays, objects...)
- Function calling and allocation

So when calculating the space complexity of a function or piece of code, I like to ask if any of the above three requirements are happening based on the size of an dynamic input value. 

If not, it's almost certainly O(1). For instance, if a new array (or object or string) is being created and it's length will be determined based on the size of a parameter, the space used by that new array is increasing at a linear rate O(n). 

To achieve quadratic O(n^2) space complexity, recursion or a similar intensive process is typically required. 

This video is a nice summary: https://www.youtube.com/watch?v=SHIg5UIfBnI