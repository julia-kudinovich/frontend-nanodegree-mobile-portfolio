
### How to run the application

Go <a href="https://julia-kudinovich.github.io/frontend-nanodegree-mobile-portfolio/" target="_blank">here</a> to open the application directly from my GitHub page.

### Optimization made to index.html
- Minified css and js files
- Optimized images
- Set js scripts to async
- Added *media="print"* to print.css
- Inlined critical css ctyles
- Loaded Google font asynchronously using Web Font Loader library and moved it to the bottom of the body tag


###Optimization made to views/js/main.js
- Moved *items* and *items.length* definitions out of the *updatePositions()* function making them global
- Moved part of the *phase* definition out of the loop in *updatePositions* to avoid layout recalculating
- Moved part of the *pizzasDiv* definition out of the loop
- Implemented *requestAnimationFrame()* function
- Reduced the number of moving pizzas to 50
- Moved document.querySelector("#movingPizzas1") outside of the for loop to avoid style recalculation
- Added *translateZ(0)* , *transform*  and *backface-visibility: hidden* to moving pizzas elements
- Optimized *resizePizzas()* function to not use *determineDx()* function and calculate size of pizzas more directly
- Changed *document.querySelectorAll()* to *getElementsBy* method.
- Created position array to hold all the possible phases since there are only 5 unique values for phases for every scroll and we do not need to calculate them on every scroll.
- Created a varible to store length of the pizza element to avoid checking the lenght in every iteration of the loop
- Declared the elem variable in the initialisation of the for-loop  to prevent i tbeing recreated with every loop iteration
