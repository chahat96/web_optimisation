### Udacity Front End Nanodegree Project

	------Website Optimization-------
	
	
	This Project is Live At this link:- https://chahat96.github.io/web_optimisation/

### Key features of the project
	1.Index.html file of the portfolio website should have a score of 90 or more on both Desktop and Mobile
	
	2.pizza.html file should render with a consistent frame rate of 60fps.
	
	3.Time to resize pizzas is less than 5 ms using the pizza size slider on the views/pizza.html page 

### Achieved 
	1.Achieved score of index.html for the portfolio website of 96 on mobile and 97 on desktop.
	
	2.pizza.html website is working fine.
	
	3.Time to resize pizzas is less than 5ms.

### Running of project:

	1. Download the project from the github.com/chahat96.
	
	2. Unzip the compressed file.
	
	3. open the index.html file and views/pizza.html file in any browser of your choice.

	-------Optimization Done in the Project-------

### Optimization 1: 

Critical Rendering Path for the index.html of the portfolio website 

	--- Page Speeds score of the index.html is more than 90 for both Desktop and Mobile. ---

Required changes that were made in the index.html file.

	1.Added async Attribute to javascript file so that javascript file will be run asynchronously as soon as it is available. 
	Inlined CSS reduces the amount of files the browser has to download prior to displaying your web page.
	
	2.Images in the index.html file are compressed to a more suitable size and are thus optimized.
	
	3.Media attribute is added to print.css file. Media file optimized the css for a particular set of devices.
	Used for optimizing index.html for mobile.

	4.Style.css file used as inline css in index.html file.

	


### Optimization 2:

Changing the js/main.js to make views/pizza.html render with a consistent frame-rate at 60fps when scrolling.:

	---Pizza.html render with a consistent frame-rate of 60fps when scrolling  ---
	
	1. Instances of querySelector are to more efficient DOM HTML method getElementsByClassName() from getElementById().
	
	2. Caching the required DOM elements to cach, so that it saves processing power. It is space beneficial to "store it in code" or in other term cache them.
	
	3. The browser is not querying the DOM every time as document.body is out of the for loops in the changePizzaSizes() and updatePositions() functions. 

	4.Moved out the reference out of the loop so that it only need the getAdj.
	
	5. Created an additional for loop to set the element's width in the changePizzaSizes() function.
