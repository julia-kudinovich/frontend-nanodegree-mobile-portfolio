
### How to run the application

Go to <a href="https://julia-kudinovich.github.io/frontend-nanodegree-mobile-portfolio/" target="_blank">here</a> to open the application directly from my GitHub page.

### Optimization made to index.html
- minified css and js files
- optimized images
- set js scripts to async
- added style-smartphone.css to css folder and initialized it with *media = "screen and (max-width: 480px)*
- added *media="print"* to print.css
- inlined critical css ctyles
- moved style.css to the bottom of the body tag
- removed link to google font


###Optimization made to views/js/main.js
- Moved *items* and *items.length* definitions out of the *updatePositions()* function making them global
- Moved part of the *phase* definition out of the loop in *updatePositions* to avoid layout recalculating
- Implemented *requestAnimationFrame()* function
- Reduced the number of moving pizzas to 50
- Moved document.querySelector("#movingPizzas1") outside of the for loop to avoid style recalculation
- Added *translateZ(0)* and *transform* to moving pizzas elements
- Optimized *resizePizzas()* function to not use *determineDx()* function and calculate size of pizzas more directly

