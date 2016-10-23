## Website Performance Optimization portfolio project

The challenge of this project is to take an underperforming website and make its pages render as quickly as possible by applying the techniques we learned in the Udacity's [Critical Rendering Path course](https://www.udacity.com/course/ud884) course.

## Part 1: Optimize PageSpeed Insights score for index.html

The Goal: a Google PageSpeed Insights score of 90 or higher for mobile and desktop.

- Open the [live page](https://sandrine10.github.io/frontend-nanodegree-mobile-portfolio/) in your favorite browser.
Copy the URL and paste it in the analyze field at 
 [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) to view the scores
Or see it directly <a href="https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fsandrine10.github.io%2Ffrontend-nanodegree-mobile-portfolio%2F" target="_blank">here</a>

## Optimizations I made to index.html:

- Add media=“print” to print.css link
- Move CSS.style from the CSS folder to index
- Add async attribute to the Google analytics JS script
- Remove style.css
- Remove google fonts

### Optimize the following images:

- pizzeria.jpg
- pizza.png
- profilepic.jpg
- 2048.png
- cam_be_like.jpg
- mobilewebdev.jpg

## Part 2: Optimize Frames per Second in pizza.html

The Goal: Page renders at 60 frames per second when scrolling, the pizza size slider resizes pizza images in under 5ms.

- Open the [pizza page](https://sandrine10.github.io/frontend-nanodegree-mobile-portfolio/views/pizza.html) in your browser.
- Open DevTools and navigate to the Timeline.
- Switch on Profile JS and Paint.
- Press the record button at the top left, scroll a bit, then press the record button again to view the record.

## Optimizations I made to views/js/main.js:

- In line 379, 387 changed style.width to classList.add
- In line 409, 412, 415 replaced querySelector with getElementById
- In line 454 moved dx outside of the loop
- In line 455 moved calculation of newWidth outside of the loop
- In line 474 moved randomPizzas outside of the loop
- In line 506 stored item array outside of function
- In line 542 changed the number of sliding pizzas.
