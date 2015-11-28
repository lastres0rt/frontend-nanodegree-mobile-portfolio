## Website Performance Optimization portfolio project

Several optimizations have been made to this portfolio to make `index.html` achieve at least a score of 90 according to Google PageSpeed Insights, as well as optimizing `pizza.html` to run at a rate of 60 fps or better.

### How To Run It

Click this link for the [Front-End Nanodegree Mobile Portfolio](http://lastres0rt.github.io/frontend-nanodegree-mobile-portfolio/) to see `index.html`, and then click this link for [Cam's Pizzeria Page](http://lastres0rt.github.io/frontend-nanodegree-mobile-portfolio/views/pizza.html) to see `pizza.html`.

### Optimizations Made

#### index.html

1. Asynchronous loading of Google WebFont (a JS file)
1. Asynchronous loading of the Google Analytics tracker
1. Asynchronous loading of the performance tracker
1. Inlining of the CSS (to prevent round trips)
1. Image optimization of large image files, specifically `pizzeria.jpg`

#### pizza.html

1. Image optimization of large image files, specifically `pizzeria.jpg`

##### style.css
1. The addition of `will-change: transform;` to the `.mover` class

##### main.js

1. Reduced the number of pizzas needed in the background from 200 down to a dynamically-selected number based on `window.innerHeight`
2. Optimized the `updatePostions` function to reduce the number of calculations and functions being made within the iteration loop, especially `scrollTop`
3. Optimized the `changePizzaSizes(size)` function to reduce the number of calculations and functions being made within the iteration loop.