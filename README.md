## Website Performance Optimization portfolio project

The goal of this project is to take an underperforming website and make its pages render as quickly as possible by applying the techniques learned Udacity's [Critical Rendering Path course](https://www.udacity.com/course/ud884) course.

##Steps to run project successfully

###PageSpeed

- Open the [live page](https://sandrine10.github.io/frontend-nanodegree-mobile-portfolio/) in your favorite browser.

- Then in a separate browser tab, go to [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) and type in the same URL that you used to open the live page. This should show my PageSpeed Insights scores. 
Or see it directly <a href="https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fsandrine10.github.io%2Ffrontend-nanodegree-mobile-portfolio%2F" target="_blank">here</a>


###Pizza.html

- Open the [pizza page](https://sandrine10.github.io/frontend-nanodegree-mobile-portfolio/views/pizza.html) in your browser.

- Open DevTools and navigate to the Timeline.

- Switch on Profile JS and Paint.

- Press the record button at the top left, scroll a bit, then press the record button again to view the record.

- Once you have reviewed the scrolling records, find the pizza resize button, press the record button again, click the resize button a few times, then press the record button again to view the record.


##Optimizations I made

###Optimizations to index.html

- Add media=“print” to print.css link
- Move CSS.style from the CSS folder to index
- Add async attribute to the Google analytics JS script
- Remove style.css
- Remove google fonts

###Optimize the following images:

- pizzeria.jpg
- pizza.png
- profilepic.jpg
- 2048.png
- cam_be_like.jpg
- mobilewebdev.jpg

###Optimizations to views/js/main.js




To get started, check out the repository and inspect the code.

### Getting started

####Part 1: Optimize PageSpeed Insights score for index.html

Some useful tips to help you get started:

1. Check out the repository
1. To inspect the site on your phone, you can run a local server

  ```bash
  $> cd /path/to/your-project-folder
  $> python -m SimpleHTTPServer 8080
  ```

1. Open a browser and visit localhost:8080
1. Download and install [ngrok](https://ngrok.com/) to the top-level of your project directory to make your local server accessible remotely.

  ``` bash
  $> cd /path/to/your-project-folder
  $> ./ngrok http 8080
  ```

1. Copy the public URL ngrok gives you and try running it through PageSpeed Insights! Optional: [More on integrating ngrok, Grunt and PageSpeed.](http://www.jamescryer.com/2014/06/12/grunt-pagespeed-and-ngrok-locally-testing/)

Profile, optimize, measure... and then lather, rinse, and repeat. Good luck!

####Part 2: Optimize Frames per Second in pizza.html

To optimize views/pizza.html, you will need to modify views/js/main.js until your frames per second rate is 60 fps or higher. You will find instructive comments in main.js. 

You might find the FPS Counter/HUD Display useful in Chrome developer tools described here: [Chrome Dev Tools tips-and-tricks](https://developer.chrome.com/devtools/docs/tips-and-tricks).

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
