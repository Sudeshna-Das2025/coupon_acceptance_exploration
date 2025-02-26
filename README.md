# Will the Customer Accept the Coupon?


## Context

This application explores a dataset in UCI Machine Learning Repository that was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, and passenger, and then asks people whether they will accept different types of coupons if they are the driver. Coupons offered are for cheap restaurants (that cost $20/person), coffee houses, carry outs, bars, and expensive restaurants (that cost $20-$50/person). This application explores various factors that influence a driver's decision in accepting a coupon and seeks to understand differences between drivers who accepted different coupons vs. those who did not. 


## Data
Link to dataset is provided below:
https://archive.ics.uci.edu/dataset/603/in+vehicle+coupon+recommendation

A [copy of the data](/data/coupons.csv) is also uploaded in this repository under the data folder.


## Data Description
The attributes of this data set include:

**User attributes**

* Gender: male, female

* Age: below 21, 21 to 25, 26 to 30, etc.
* Marital Status: single, married partner, unmarried partner, or widowed
* Number of children: 0, 1, or more than 1
* Education: high school, bachelors degree, associates degree, or graduate degree
* Occupation: architecture & engineering, business & financial, etc.
* Annual income: less than $12500, $12500 - $24999, $25000 - $37499, etc.
* Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
* Number of times that he/she buys takeaway food: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
* Number of times that he/she goes to a coffee house: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
* Number of times that he/she eats at a restaurant with average expense less than $20 per person: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
* Number of times that he/she goes to a bar: 0, less than 1, 1 to 3, 4 to 8 or greater than 8


**Contextual attributes**

* Driving destination: home, work, or no urgent destination
* Location of user, coupon and destination: we provide a map to show the geographical location of the user, destination, and the venue, and we mark the distance between each two places with time of driving. The user can see whether the venue is in the same direction as the destination.
* Weather: sunny, rainy, or snowy
* Temperature: 30F, 55F, or 80F
* Time: 10AM, 2PM, or 6PM
* Passenger: alone, partner, kid(s), or friend(s)


**Coupon attributes**

* time before it expires: 2 hours or one day

