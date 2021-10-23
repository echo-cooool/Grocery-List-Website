# COMP3019J Assignment

### Project: Grocery List Website

### Team Members:

* Wang Yuyang 19206226
* Yang Liuxin 19206207

### Project Description
The website should allow multiple grocery shops to set up products available, along with their unit prices as well as images. 
The website should allow users to visit different shops, and put items into their basket. The website should allow users to view their basket at all times, and add/remove items from the basket. 
The website should allow users to increase/ decrease the quantity of the items while looking at their baskets. 
It should also calculate the total expenditure/cost for all items in the basket. 
Finally, it should create an itemised list of the user’s shopping bill, grouped by the shop.

### Intended Functionalities
#### Common Functionalities
- [x] Allow sellers and buyers to **visit** different shops

#### Seller / Shop
- [x] Allow multiple sellers/shops to **upload** products with their prices and images
- [x] Allow sellers to **visit** different shops
- [x] Allow sellers to **manage** their **items**
- [x] Allow sellers to **manage** their **orders**

### Implemented Functions for MileStone1



### Preview this project (Deployed in Heroku)

This is a **preview version** of this project, it might contain errors or out-dated pages.
Please use python to run this project locally to see the latest website.

[http://comp3019j-web-dev.herokuapp.com/](http://comp3019j-web-dev.herokuapp.com/)


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
or

```shell
python run.py
```

or

If pipeline passed then this docker contains the same code with master:

![pipeline](https://csgitlab.ucd.ie/19206226/TEAM_20/badges/master/pipeline.svg)

```shell
docker pull echo0821/web-project:latest 
docker run -p 5000:5000 echo0821/web-project:latest
```
#### Open the web page using Firefox / Chrome / Edge
**Safari and IE is not offfically supported**

URL: http://localhost:5000

or

URL: http://127.0.0.1:5000



### User Accounts for Testing

Shopper:
* Username: shop1
* Password: 123

Buyer:
* Username: buyer1
* Password: 123

### Roles in the system
1. Buyers
   1. Register and Login in the login-register page
   2. Can add products to his shopping cart
   3. Can view his cart
   4. Can make orders 
   5. Can view his orders
   6. Cannot add products to the site
   7. Cannot manage products of the site
2. Seller (Registered by Admin, Not allowed to be created by public register)
   1. Can add products
   2. Can manage products 
   3. Can view orders made from his shop
   4. Can confirm orders
   5. **Cannot view his cart**
   6. Cannot make orders
   
### Buyer's Functionality
* Navigation bar
  * Automatically change for different roles
  * Auto hide & display flash message
* Index Page
  * Allowing buyers to view recommended products
  * Allowing buyers to view sample products grouped by shops
* Shopping Cart
  * Buyers can add product to their shopping cart
  * Items in the cart can be removed or added in quantity
  * Items can be correctly count if buyers add the product multiple times from product-details page
* Ordering
  * Buyers can make orders from his shopping cart
  * After paying, user can view the order in the order page
* User profile
  * User can change their avatar in the profile page
  * User can change their email in the profile page
  * User can change their password in the profile page

### Seller's Functionality
* Navigation bar
  * Automatically Change for different roles
  * Auto hide & display flash message
* Index Page
  * Allowing sellers to view recommended products
  * Allowing sellers to view sample products grouped by shops
* Product Management
  * Sellers can add product to the system
  * Sellers can modify product of the system
  * Sellers can remove product from the system
* Order Management
  * User can view the orders made in his shop 


### Characteristic

* Responsive Layout (flex Layout)
* Allowing unregistered user to view products
* Auto redirect to login page
* CSRF Protection
* Blueprint for routing


### TODO
* Navigation bar
  * 
* Index Page
  * 
* Shopping Cart
  * 
* Ordering
  * 
* User profile
  * 
* Product Management
  * 
* Order Management
  * 
