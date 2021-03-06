#Website Performance Optimization portfolio project
![Part of the Udacity Front-End Web Development Nanodegree](https://img.shields.io/badge/Udacity-Front--End%20Web%20Developer%20Nanodegree-02b3e4.svg)

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
1. The addition of `will-change: transform;` to the `.randomPizzaContainer` class

##### main.js

1. Reduced the number of pizzas needed in the background from 200 down to a dynamically-selected number based on `window.innerHeight`
1. Optimized the `updatePostions` function to reduce the number of calculations and functions being made within the iteration loop, especially `scrollTop`
1. Optimized the `changePizzaSizes(size)` function to reduce the number of calculations and functions being made within the iteration loop.
1. Replaced instances of `querySelector()` with `getElementById()`
1. Replaced instances of `querySelectorAll()` with `getElementsByClassName()`
1. Refactored `changePizzaSizes(size)` to remove unnecessary functions and document calls.
