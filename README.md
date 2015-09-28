# Udacity Data Visulization

## Summary

This project is to create a data visulization for the Kaggel's Titanitc data set. Everything is inside the index.html file. To open it, just use a web browser the graphs will show up. The purpose of the graphs is to show how different sub groups of the passengers had different final results, such as the price of the tickets, whether or not survived, and so on. 

## Design

All of the graphs are generated using dimple.js, which is a javascript library on top of d3.js. I decided to use dimple.js rather than the low level d3.js because it is much simpler to use, and would allow me to quickly generate the plots that I wanted. Altough d3.js might provide more flexibilities, but since the data set used in this example is not so complicated, and the main point of interests is to compare the different results between different social groups, I decided to use dimple.js. Note that the first graph is similar to the fourth one, except that the fourth one is an all-in-one graph, including 4 variables: Age as in x-axis, Fare as in y-aixs, pclass as in legend, and the size of the circles with 0 for unsurvived, and 1 for survived. 

## Feedback

### Feedback 1: I don't understand the y axis for some of the plots.
### Modification 1: Dimple.js use a aggregateMethod of sum by default, which in most of the cases here doesn't make sense. That caused some confusion at first. So I used instead avg method for aggregation. For example, in the "Sex vs Survivded" bar plot, the avg method essentailly gives a percentage of how many female or male passangers survived. This type of plot include: "Age vs Survived", "Sex vs Survived", "Pclass vs Survived", "SibSp vs Survived", "Parch vs Survived". Some other plots, using the same avg method, gives information about the average value for a certain category. These include: "Sex vs Age" with average age for each gender, "Sex vs Pclass" with average Pclass, "Embarked vs Pclass" with average Pclass.

### Feedback 2: You have constructed plots with two variables, and more than 2 variables, how about plots with only one variable?
### Modification 2: Some times plots with one variable also provide important statistical information, for example histogram plots. So I added some of the important one variable plots, such as the bar plots of Survived people, Pclasses, etc. 

### Feedback 3: The first two plots can be combined into a single plot
### Modification 3: The first plot, which is a plot with 4 variables (Age, Fare, Plcass, Survived), was initially given by two seperate plots: (Age, Fare, Pclass) and (Age, Fare, Survived). Then I found Dimple.js provide a size option for the z axis. So I decided to use legends to represent the Pclass variable, and different size of the circles to represent the Survived variable. 


## Resources

dimple.js: http://dimplejs.org/  
d3.js: http://d3js.org/
