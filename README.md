## Intallations
The librarys used in this project are:
* pandas
* numpy
* matplotlib
* sys
* seaborn
* sklearn



## Project Motivation

This project has two main goals.
The first one is to get some insights from the Airbnb Madrid dataset. To do this, I have applied the CRISP-DM method.

The dataset is full of information about the accommodations available on Airbnb in the city of Madrid. With all this information, we are going to ask ourselves a few questions:

Q1.-Is the quantity of accommodation offered equal all around Madrid?

Q2.-If a neighborhood group has a lot of accommodations, does it mean that each of its individual neighborhoods has them too? 

Q3.-Are the prices equal all over Madrid? 

Q4.-How are the prices and availability rates in Madrid over the next few months? 

Q5.-Finally, how well can we predict prices based on the rest of the features? For this task, I will fit a linear model that will estimate the price based on other features.

The second goal is to learn how to apply all the information and techniques I have learned so far to a real case.

## Results

This project has been structured using the CRISP-DM method. In the notebook file, you will find it easy to go through each step since everything is documented.

1.- Business Understanding
  In this part, I first took a look at the data provided by Airbnb. Everyone can find this dataset in the [Airbnb get-data](http://insideairbnb.com/get-the-data/)
  After understanding what each feature meant, I came up with some ideas.

2.- Data Understanding
  Now, it was time to take a look at the types of variables in each column, the shape of each dataframe, and take a look at the null values.

3.- Data Preparation
  In this part, I drop the columns with more than 50% of Nan values and some others that weren't useful for this project. After that, I corrected some data types and nomenclature errors. 
  
4.- Data Modelling
  At that point, a linear model is created.
  
5.-Result evaluation
  In this part, the model was evaluated. Since the value of the r-square is 0.5234, we cannot say that we can predict or estimate the price of an accommodation based on the other selected features. A r-square of 0.75 or more will be enough.


#### Answers to que questions

A1.- Each bar in the plot represents a neighborhood group in Madrid. The plot shows the percentage of accommodations in that neighborhood. For example, more than the 40% of the accommodations available in Airbnb Madrid are located in the neighborhood "Centro", which in English means the center of the city. So the answer to the questions is no. But, we have 2  features. First, we have a neighborhood group, and then we have a neighborhood. A neighborhood group is formed by some neighborhoods. This is important for the next question.

A2.- Since we don't get the same rainbow pattern, the answer is no. However, each neighbourhood that belongs to the center zone has a lot to offer. So this answer will be true for the center zone only. The rest is divided into the rest of the neighbourhoods.

A3.- The prices are not equal all around Madrid. Based on the first bar plot, we can see that the mean price of the accommodation depends a lot on the neighborhood group. We can also see, thanks to the box plot, that the range of prices is different for different neighbourhood groups in Madrid.

A4.-We can see that the prices and availability rate seem to be dependent on the month. People seem to visit Madrid more in the winter and spring months. This can be due to the hot weather Madrid experiences in the summer months. The month with the highest availability rate is also the cheapest. This can be caused by the offer and demand effect.

A5.- Not very well..., that was explained earlier.



## File descriptions

Thre are only 2 main files, the first one, a jupyter notebook with all the project. Along this one, you will find a .py file, inside you will find some functions I created to be used in this project.

## Author 
Pablo Carbonero Álvarez
