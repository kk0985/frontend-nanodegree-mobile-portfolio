## Website Performance Optimization portfolio project

================================
Optimization Testing
	- set up GitHub Page http://kk0985.github.io/frontend-nanodegree-mobile-portfolio/
	  after attempt to use python and ngrok failed
		*set up of python and opening localhost:8080 worked as expected
		*could not figure out how to add command code for ngrok in git bash after python -m SimpleHTTPServer 8080 and opening browser so I used ngrok application, which did not provide a public URL.  This led me to use gh-pages.

1) Optimize index.html to 90 for mobile and desktop
	- personalized to my name and added my pic
	- changed link href for Open Sans to a Style tag
	- relocated script for GoogleAnalytics to before close body tag
	- Pagespeed Insight has optimization at 87/100 for mobile and 93/100 for desktop

2) Optimize pizza.html to 60fps
	- personalized to my name and added my favorites
	- changes made to views/js/main.js
		* moved var for randomPizzaContainer out of function for changePizzaSizes
		* requestAnimationFrame implemented for background pizzas as seen on html5rocks
		* function for updatePositions - changed items[i].style.lft to transform and translate
		* moved items variable to end to make it available globally
	- changes made to views/css/main.css
		* added will-change: transform and transform: translateZ(0) to .mover
	- changes made to views/images/pizzeria.jpeg
	    * compressed and resized to 64KB from 2.3MB

3) Optimized css/style.css using CSS Beautifier at html.fwpolice.com/css

4) Optimized index.html and pizza.html using Format HTML for Free at www.cleancss.com/html-beautify/
==================================

How to run the app:
	open index.html in your browser

