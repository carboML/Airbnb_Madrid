## Intallations
The librarys used in this project are:
* pandas
* numpy
* matplotlib
* sys
* seaborn
* sklearn



## Project Motivation

This project has 2 main goals. The first one is to get some insigths from the Airbnb Madrid dataset. To do this, I have applied the CRISP-DM method.

The dataset is full of information about the accommodates avaible in Airbnb in the city of Madrid. With all this information we are going to ask ourself a few questions:

Q1.- Is the quantity of accommodation offer equal all arround Madrid? <br>
Q2.- If a neighbourhood group has a lot of accommodations, does it mean that each of it's indiviual neighbourhood has it too? <br>
Q3.- Are the prices equal all over Madrid <br>
Q4.- How are the prices and availability rate in Madrid over the months <br>
Q5.- Finally, how well can we predict price based on the rest of the feautures? For this task, I will fit a linear model that will estimate the price based on other features <br>

The second goal is to learn how to apply all the information and techniques I have learn so far to a real case.

## Results

This project has been structured using the CRISP-DM method. In the notebook file you will find easy to go throgth each step since everything is documented.

1.- Business Understanding
  In this part, I first took a look at the data provided by Airbnb. Everyone can find this dataset in the [Airbnb get-data](http://insideairbnb.com/get-the-data/)
  After understand what does each feature means I came up with some ideas.

2.- Data Understanding
  Now, it was time to take a look to the type of variables of each column, the shape of each dataframe and take a look at the null values.

3.- Data Preparation
  In this part I drop the columns with more than 50% of Nan valules and drop some column that weren't useful for this project. After that, I corrected some data types and nomenclature errors. 
  
4.- Data Modelling
  At tis point, a linear model was created.
  
5.-Result evaluation
  In this part the model was evaluated. Since the value of the r-square is 0.5234 we cannot say that we can predict or estimate the price of an accomodating based on the other selected features. A r-square of 0.75 or more will be enougth.


# Answers to que questions

A1.- Each bar of the plot represent a neighborhood group in Madrid. The plot show the percentaje of accomodations in that neighborhood. For example, more than the 40% of the accomodations available in Airbnb Madrid are located in the neighborhood "Centro", which in English mean, center of the city. So the answer for the questions is no. But, we have 2 features, first we have neighborhood group and then we have neighborhood. A neighborhood group form by some neighborhood. This is important for the next question.

A2.- Since we don't get the same rainbow pattern, the answer is no. However, each neighbourhood that belong to the center zone, has a lot of offer each. So this answer will be true for the center zone, the rest is divided into the rest of neighbourhoods.

A3.- The prices are not equal all arround Madrid. Based on the first bar plot, we can see that the mean price of the accommodations depends a lot on the neighbourhood group. We also can see, thanks to the box plot that the range of prices are different for different neighbourhoods groups in Madrid

A4.-We can see that the prices and availabillity rate seem to be depent on the month. People seem to visit Madrid more on the Winter and Spring months. This can be due to the hot weather Madrid experiment in the Summer months. The month with more availability rate is also the cheaper, this can be cause to offer and demand effect.

A5.- Not very well..., that was explained earlier



## File descriptions

Thre are only 2 main files, the first one, a jupyter notebook with all the project. Along this one, you will find a .py file, inside you will find some functions I created to be used in this project.

## Author 
Pablo Carbonero Álvarez
