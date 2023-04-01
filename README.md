# Diamond price predictor.
![Diamond](Images/Diamond.png)

## Introduction.
---
The predictive models i made are for a kaggle competition where the objective is to predict acurately the price of a set of diamonds.

## How?
---

We have a csv with diamonds with many characteristics like it's color, carat, clarity etc. Aswell we have the prices of these diamonds, so we can train our models with this data to try to predict then the test diamonds, which we have all of it's characteristics except it's price.
So that's the objective, acurately predict diamond prices.

## My prediction models.
---

I got two models that had very good metrics, so i'll explain briefly how they work.

Model_1: The objective for this model was to have as few columns to predict as posible, so i made an exhaustive analysis of every column and droped the ones that were not relevant.
![xyz](Images/xyz.png).

As we can see in this graph the numeric columns carat, x, y and z are very related to the predictive variable price, so i decided to drop x,y and z becouse carat englobes all of these three as its the weight of the diamond, so it's obvious that a heavier diamond is larger, x, y and z represent it's millimeters in length.

I droped depth and table aswell becouse they were not very related to the price of the diamond and my objective was to have as few variables as possible to predict the price.


![carat_outlier](Images/carat_out.png)


In this first model i did a robust standardization becouse it had many outliers that i didn't want to replace or erase.

!["Model"](Images/Model.png)

As we can see in this graph the least overfitted model is the Gradient Booster, and it has the best RMSE of them all. So i decided to use that model.



