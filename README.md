# About Drover

Drover is a VC-backed, growth-stage marketplace company offering monthly, all-in car subscriptions to customers who want to experience car ownership as it should be: digital, flexible and at a fair, transparent price. For some more detail, check out our press coverage in TechCrunch, Forbes or CityAM.

We want to build ever more extraordinary digital experiences for our users and we need your help: come on board and join our 20-strong engineering team busy changing the automotive landscape.

# Cars
As you know Drover is an online marketplace for booking cars, and as you expect we try to have as much cars as we can on our platform. For this challenge we want you to implement a REST API to store, update and list cars.

A car's make is the brand of the vehicle, while the model refers to the name of a car product and sometimes a range of products. For example, Toyota is a car make and Yaris is a car model. So for each car we will create on the challenge we will need to have the following properties:
* Make
* Model
* Year
* Color
* Monthly price

For this challenge only consider the following Makes and Models:
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

Create a service with some REST APIs that would allow to create, update and list cars. It's up to you to decide the stack you want to use and how far do you want to go.

The challenge must have the following 5 requirements implemented:

1) Create a REST endpoint to create a car in one POST request

`PUT /cars/{id}`

```json
{
   "make": "toyota",
   "model": "yaris",
   "year": 2015,
   "color": "red",
   "price": {
       "amount": 50000,
       "currency_code": "EUR"
   }
}
```

2) Create an endpoint to update a car.

`PUT /cars/{id}`

```json
{
   "make": "toyota",
   "model": "yaris",
   "year": 2015,
   "color": "red",
   "price": {
       "amount": 50000,
       "currency_code": "EUR"
   }
}
```

3) Create an endpoint to fetch all cars. The results *should be sorted* by price from low to high.

`GET /cars`

```json
{
   "cars": [
      {
         "id": 1,
         "make": "toyota",
         "model": "yaris",
         "year": 2015,
         "color": "red",
         "price": {
             "amount": 40000,
             "currency_code": "EUR"
         }
      },
      {
         "id": 2,
         "make": "bmw",
         "model": "x1",
         "year": 2017,
         "color": "black",
         "price": {
             "amount": 60000,
             "currency_code": "EUR"
         }
      }
   ]
}
```

5) Add on the GET cars endpoint the possibility to filter by make and/or color. On the example showed on point 3 if we wanted to get all cars from toyota and red the response should be:

```json
{
   "cars": [
      {
         "id": 1,
         "make": "toyota",
         "model": "yaris",
         "year": "2015",
         "color": "red",
         "price": {
             "amount": 40000,
             "currency_code": "EUR"
         }
      }
   ]
}
```

## Bonus Points

6) On the GET cars API add the possibility to do pagination, showing 20 cars at a time

------

## Questions?

If you have any problems or questions please reach out to us at techleads@joindrover.com

