# Udacity Data Visulization

## Summary

This project is to create a data visulization for the Kaggel's Titanitc data set. Everything is inside the index.html file. To open it, just use a web browser the graphs will show up. The purpose of the graphs is to show how different sub groups of the passengers had different final results, such as the price of the tickets, whether or not survived, and so on. 

## Design

All of the graphs are generated using dimple.js, which is a javascript library on top of d3.js. I decided to use dimple.js rather than the low level d3.js because it is much simpler to use, and would allow me to quickly generate the plots that I wanted. Altough d3.js might provide more flexibilities, but since the data set used in this example is not so complicated, and the main point of interests is to compare the different results between different social groups, I decided to use dimple.js. Note that the first graph is similar to the fourth one, except that the fourth one is an all-in-one graph, including 4 variables: Age as in x-axis, Fare as in y-aixs, pclass as in legend, and the size of the circles with 0 for unsurvived, and 1 for survived. 

## Feedback



## Resources

dimple.js: http://dimplejs.org/
d3.js: http://d3js.org/
