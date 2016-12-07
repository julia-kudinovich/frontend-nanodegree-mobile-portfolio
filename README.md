
### How to run the application

Go to <a href="https://julia-kudinovich.github.io/frontend-nanodegree-mobile-portfolio/" target="_blank">here</a> to open the application directly from my GitHub page.

### Optimization made to index.html
- Minified css and js files
- Optimized images
- Set js scripts to async
- Added style-smartphone.css to css folder and initialized it with *media = "screen and (max-width: 480px)*
- Added *media="print"* to print.css
- Inlined critical css ctyles
- Moved style.css to the bottom of the body tag
- Loaded Google font asynchronously using Web Font Loader library and moved it to the bottom of the body tag


###Optimization made to views/js/main.js
- Moved *items* and *items.length* definitions out of the *updatePositions()* function making them global
- Moved part of the *phase* definition out of the loop in *updatePositions* to avoid layout recalculating
- Implemented *requestAnimationFrame()* function
- Reduced the number of moving pizzas to 50
- Moved document.querySelector("#movingPizzas1") outside of the for loop to avoid style recalculation
- Added *translateZ(0)* and *transform* to moving pizzas elements
- Optimized *resizePizzas()* function to not use *determineDx()* function and calculate size of pizzas more directly

