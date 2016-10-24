# Website Performance Optimization portfolio project

The challenge of this project is to take an underperforming website and make its pages render as quickly as possible by applying the techniques we learned in the Udacity's [Critical Rendering Path course](https://www.udacity.com/course/ud884) course.

## Part 1: Optimize PageSpeed Insights score for index.html

The Goal: a Google PageSpeed Insights score of 90 or higher for mobile and desktop.

- Open the [live page](https://sandrine10.github.io/frontend-nanodegree-mobile-portfolio/) in your favorite browser.
Copy the URL and paste it in the analyze field at 
 [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) to view the scores
Or see it directly <a href="https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fsandrine10.github.io%2Ffrontend-nanodegree-mobile-portfolio%2F" target="_blank">here</a>

### Optimizations I made to index.html:

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

### Optimizations I made to views/js/main.js:

- In line 379, 387 changed style.width to classList.add
- In line 409, 412, 415 replaced querySelector with getElementById
- In line 454 moved dx outside of the loop
- In line 455 moved calculation of newWidth outside of the loop
- In line 474 moved randomPizzas outside of the loop
- In line 506 stored item array outside of function
- In line 515 moved out the document.body.scrollTop from the loop and created a variable
- In line 519 replaced document.body.scrollTop with the new variable
- In line 542 changed the number of sliding pizzas.
- In line 547 increased the number of sliding pizzas

### Getting started

Some useful tips to help you get started:

1. Check out the repository
1. To inspect the site on your phone, you can run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ngrok 8080
  ```

1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights! [More on integrating ngrok, Grunt and PageSpeed.](http://www.jamescryer.com/2014/06/12/grunt-pagespeed-and-ngrok-locally-testing/)

Profile, optimize, measure... and then lather, rinse, and repeat. Good luck!

### Optimization Tips and Tricks
* [Optimizing Performance](https://developers.google.com/web/fundamentals/performance/ "web performance")
* [Analyzing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/analyzing-crp.html "analyzing crp")
* [Optimizing the Critical Rendering Path](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/optimizing-critical-rendering-path.html "optimize the crp!")
* [Avoiding Rendering Blocking CSS](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/render-blocking-css.html "render blocking css")
* [Optimizing JavaScript](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/adding-interactivity-with-javascript.html "javascript")
* [Measuring with Navigation Timing](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/measure-crp.html "nav timing api"). We didn't cover the Navigation Timing API in the first two lessons but it's an incredibly useful tool for automated page profiling. I highly recommend reading.
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/eliminate-downloads.html">The fewer the downloads, the better</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/optimize-encoding-and-transfer.html">Reduce the size of text</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/image-optimization.html">Optimize images</a>
* <a href="https://developers.google.com/web/fundamentals/performance/optimizing-content-efficiency/http-caching.html">HTTP caching</a>

### Customization with Bootstrap
The portfolio was built on Twitter's <a href="http://getbootstrap.com/">Bootstrap</a> framework. All custom styles are in `dist/css/portfolio.css` in the portfolio repo.

* <a href="http://getbootstrap.com/css/">Bootstrap's CSS Classes</a>
* <a href="http://getbootstrap.com/components/">Bootstrap's Components</a>

### Sample Portfolios

Feeling uninspired by the portfolio? Here's a list of cool portfolios I found after a few minutes of Googling.

* <a href="http://www.reddit.com/r/webdev/comments/280qkr/would_anybody_like_to_post_their_portfolio_site/">A great discussion about portfolios on reddit</a>
* <a href="http://ianlunn.co.uk/">http://ianlunn.co.uk/</a>
* <a href="http://www.adhamdannaway.com/portfolio">http://www.adhamdannaway.com/portfolio</a>
* <a href="http://www.timboelaars.nl/">http://www.timboelaars.nl/</a>
* <a href="http://futoryan.prosite.com/">http://futoryan.prosite.com/</a>
* <a href="http://playonpixels.prosite.com/21591/projects">http://playonpixels.prosite.com/21591/projects</a>
* <a href="http://colintrenter.prosite.com/">http://colintrenter.prosite.com/</a>
* <a href="http://calebmorris.prosite.com/">http://calebmorris.prosite.com/</a>
* <a href="http://www.cullywright.com/">http://www.cullywright.com/</a>
* <a href="http://yourjustlucky.com/">http://yourjustlucky.com/</a>
* <a href="http://nicoledominguez.com/portfolio/">http://nicoledominguez.com/portfolio/</a>
* <a href="http://www.roxannecook.com/">http://www.roxannecook.com/</a>
* <a href="http://www.84colors.


