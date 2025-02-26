# Will the Customer Accept the Coupon?


## Context

This Jupyter Notebook application explores a dataset in UCI Machine Learning Repository that was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios, including the destination, current time, weather, and passenger, and then asks people whether they will accept different types of coupons if they are the driver. Coupons offered are for cheap restaurants (that cost $20/person), coffee houses, carry outs, bars, and expensive restaurants (that cost $20-$50/person). This application explores various factors that influence a driver's decision in accepting a coupon and seeks to understand differences between drivers who accepted different coupons vs. those who did not. 


## Data
Link to dataset is provided below:
https://archive.ics.uci.edu/dataset/603/in+vehicle+coupon+recommendation

A [copy of the data](/data/coupons.csv) is also uploaded in this repository under the data folder.


## Data Description
The attributes of this data set include:

**User attributes**

* Gender: male, female

* **Age**: below 21, 21 to 25, 26 to 30, etc.
* **Marital Status**: single, married partner, unmarried partner, or widowed
* **Number of children**: 0, 1, or more than 1
* **Education**: high school, bachelors degree, associates degree, or graduate degree
* **Occupation**: architecture & engineering, business & financial, etc.
* **Annual income**: less than $12500, $12500 - $24999, $25000 - $37499, etc.
* **Number of times that he/she goes to a bar**: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
* **Number of times that he/she buys takeaway food**: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
* **Number of times that he/she goes to a coffee house**: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
* **Number of times that he/she eats at a restaurant with average expense less than $20 per person**: 0, less than 1, 1 to 3, 4 to 8 or greater than 8
* **Number of times that he/she goes to a bar**: 0, less than 1, 1 to 3, 4 to 8 or greater than 8


**Contextual attributes**

* **Driving destination**: home, work, or no urgent destination 
* **Location of user, coupon and destination**: we provide a map to show the geographical location of the user, destination, and the venue, and we mark the distance between each two places with time of driving. The user can see whether the venue is in the same direction as the destination.
* **Weather**: sunny, rainy, or snowy
* **Temperature**: 30F, 55F, or 80F
* Time: 10AM, 2PM, or 6PM
* Passenger: alone, partner, kid(s), or friend(s)


**Coupon attributes**

* time before it expires: 2 hours or one day


## Key Findings from the exploration

**Observation for Bar coupon acceptance**

* Those drivers who visited bars more than 4 times a month have a much higher rate of bar coupon acceptance (approximately 77% vs. 37%) than those drivers who visited the bar 3 or less times a month

* Those drivers who visited bars more than once a month and over 25 years age have a higher rate (69.5% vs 33.5%) of bar coupon acceptance than those drivers who were not meeting the conditions and yet received bar coupons

* Those drivers who went to bar more than once a month and had passengers who are not kids and had occupations other than Farming Fishing & Forestry and received bar coupon have a higher rate of bar coupon acceptance (approximately 71.3% vs. 29.6%)than those drivers who were not meeting the conditions and yet received bar coupons

* Those drivers meeting the following conditions have a higher rate of bar coupon acceptance (approximately 59% vs. 29.8%)than those drivers who are not meeting the conditions and yet received bar coupons

	* go to bars more than once a month, had passengers that were not a kid, and were not widowed OR
	* go to bars more than once a month and are under the age of 30 OR
	* go to cheap restaurants more than 4 times a month and income is less than 50K.


**Observation for Coffee House coupon acceptance**

* Those drivers went to visit coffee houses 1 to 3 times a month have a higher rate of bar coupon acceptance (approximately 65.4% vs. 45.98%) than those drives who have never been to coffee houses.

* Those drivers who went to coffee house more than once a month and are single and received coffeehouse coupon) have a higher rate of coffeehouse coupon acceptance (approximately 67.8% vs. 45.4%)than those drivers who are not meeting the conditions and yet received coffee house coupons

* Those drivers who were employed and in Healthcare support have higher coffee house coupon acceptance rate that those who were retired (69.83% vs.45.86%)


