# COMP3019J Assignment

### Project: Grocery List Website

### Team Members:

* Wang Yuyang 19206226
* Yang Liuxin 19206207

### Introduction

The website should allow multiple grocery shops to set up products available, along with their unit prices as well as images. 
The website should allow users to visit different shops, and put items into their basket. The website should allow users to view their basket at all times, and add/remove items from the basket. 
The website should allow users to increase/ decrease the quantity of the items while looking at their baskets. 
It should also calculate the total expenditure/cost for all items in the basket. 
Finally, it should create an itemised list of the user’s shopping bill, grouped by the shop.


### Run this project

#### Set up environment
1. Install Python3.9
2. Using the following code to set up environment
```shell
python -V  # Print out python version for debugging
pip install virtualenv
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

#### Run this web sever

```shell
flask run
```

### Roles in the system
1. Buyers
   1. Register in login page
   2. Can add product to his cart
   3. Can view his cart
   4. Can Make orders 
   5. Can view his orders
   6. Can't Add products
   7. Can't Manage products
2. Seller (Registered by Admin)
   1. Can Add products
   2. Can Manage products 
   3. Can view orders from his shop
   4. Can't view his cart
   5. Can't make orders
   
### Functionality
* Navigation bar
  * Automatically Change for different role
  * Auto hide & display flash message
* Index Page
  * Allowing user to view top-selling products
  * Allowing user to view products grouped by shops

### Characteristic

* Responsive Layout
* Allowing unregistered user to view products
* Auto redirect to login page
* CSRF Protection
* High-Performance Page Caching
* Blueprint for routing


### TODO