<img src="./static/drover-logo.svg" width="200">

# Backend Challenge
## About Us

[Drover](http://joindrover.com/) is a VC-backed, growth-stage marketplace company offering monthly, all-in car subscriptions to customers who want to experience car ownership as it should be: digital, flexible and at a fair, transparent price. For some more detail, check out our press coverage in TechCrunch, Forbes or CityAM.

We want to build ever more extraordinary digital experiences for our users and we need your help: come on board and join our 20-strong engineering team busy changing the automotive landscape.

## Cars
As you know Drover is an online marketplace for booking cars, and as you expect we try to have as much cars as we can on our platform. For this challenge we want you to implement a REST API to store, update and list cars.

A car's maker is the brand of the vehicle, while the model refers to the name of a car product and sometimes a range of products. For example, Toyota is a car maker and Yaris is a car model. So for each car we will create on the challenge we will need to have the following properties:
* Maker
* Model
* Year
* Color
* Monthly, subscription price
* Available from, when the car is available for booking

For this challenge only consider the following Makers and Models:
* BMW
  * Series3
  * X1
* Toyota
  * Yaris
  * RAV4
* Renault
  * Clio
  * Megane

## What do we expect from you?
Code is your 1st class citizen.

* Good documentation.
* Good design decisions.
* Testable code.

The challenge must have the following 5 endpoints implemented:

1. Create a REST endpoint to create a `car` in one POST request
1. Create an endpoint to update a `car`.
1. Create an endpoint to fetch all `cars`. The results *should be sorted* by price from lowest to highest by default and all cars with an available from bigger than three months in the future should be filtered.
1. Add on the GET cars endpoint the possibility to filter by maker and/or color. On the example showed on point 3, if we wanted to get all cars from toyota and with red color, the response should be:

## Bonus Points

1. Possibility to do pagination, showing 20 cars at a time
1. On the GET cars API add the possibility to do a sort by price, year, maker or availability
1. Add documentation to all endpoints

------

