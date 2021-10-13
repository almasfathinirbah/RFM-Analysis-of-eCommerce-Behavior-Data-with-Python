# **E-Commerce Behavior Data from Multi Category Store with Python**

## **Business Understanding**

* E-Commerce is a business model that lets firms and individuals buy and sell things over the internet.

* This case has some business question using the data:
* What is the best product to sell in the specific time of the day?
* What is the best Event to predict that User most likely to buy a product?
* How is the behaviour of our repeat user vs new user?

## **Data Understanding**

* Behavior data for October 2019 from a large multi-category online store. Each row in the file represents an event. All events are related to products and users. Each event is like many-to many relation between products and users.

* Source Data: https://www.kaggle.com/mkechinov/ecommerce-behavior-data-from-multi-category-store

* Data Dictionary:

* event_time: Time when event happened at (in UTC).

* event_type: Only one kind of event: purchase.

* product_id: ID of a product

* category_id: Product's category ID


* category_code: Product's category taxonomy (code name) if it was possible to make it. Usually present for meaningful categories and skipped for different kinds of accessories.

* brand: Downcased string of brand name. Can be missed.

* price: Float price of a product. Present.

* user_id: Permanent user ID.

* user_session: Temporary user's session ID. Same for each user's session. Is changed every time user come back to online store from a long pause.

## **Data preparation**

* Code Used:
* Python Version: 3.7.6
* Packages: Pandas, Numpy and Matplotlib.

## **Data Cleansing**

* Check for each column and find if any column is redundant or useless.
* Check for missing values.
* Check for outliers.
* Check if the data format is already suitable for algorithm.
* Check for value that are not consistent with general common sense.

## **Exploratory Data Analysis**
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights from the pivot tables.

### **The best product to sell in the specific time of the day.**

![day 1](https://user-images.githubusercontent.com/75175081/126055622-72f3e776-1abf-4fe8-9e5d-a1a284618dd3.png)

Most consumers shop at e-commerce on Wednesday. Actually, consumers have seen the product since Sunday. After Sunday consumers are still considering whether to buy or not. Beside that consumers are still comparing one product to another. The final decision to buy is mostly made on Wednesday. The e-commerce business team can provide a campaign to convince customers. The campaign can be intensified on Wednesday.

### **The best Event to predict that User most likely to buy a product.**

![brand 1](https://user-images.githubusercontent.com/75175081/126055688-36261382-7fcf-4700-b638-5bf981668b61.png)

The best Event to predict that User most likely to buy a product is purchase of brand Samsung. Many consumers choose brand Samsung because it already has a strong and positive image for the smartphone segment. Samsung also has a simple and trend-following model. In addition, Samsung is diligent in innovating and releasing the latest technology. Seeing Samsung's very large consumer market, the e-commerce business team can make bundling package promos to expand the market.

### **The behaviour of our repeat user vs new user by category product.**

* The behavior of repeat user by category product

![repeat user 1](https://user-images.githubusercontent.com/75175081/126055747-42dbc820-d78d-42e6-9e3c-0638ff6d9e75.png)

Most repeat users buy smartphone electronics products. Meanwhile product electronics audio headphones have a very large gap. The e-commerce business team can make product bundling between electronics smartphone products and electronics audio headphones to increase profits from product categories that are still low in orders.

* The behavior of new user by category product

![new user 1](https://user-images.githubusercontent.com/75175081/126055765-f1c3dbb9-d905-44b7-9365-198e4bcfbd44.png)

Most new users buy smartphone electronics products. The e-commerce business team can make promo of this product category to attract more new market users.

## *Summary*

* Most consumers shop at e-commerce on Wednesday. The e-commerce business team can provide a campaign to convince customers. The campaign can be intensified on Wednesday.
* Many consumers choose brand Samsung because it already has a strong and positive image for the smartphone segment. The e-commerce business team can make bundling package promos to expand the market.
* Most repeat users buy smartphone electronics products. Meanwhile product electronics audio headphones have a very large gap. The e-commerce business team can make product bundling between electronics smartphone products and electronics audio headphones to increase profits from product categories that are still low in orders.
* Most new users buy smartphone electronics products. The e-commerce business team can make promo of this product category to attract more new market users.


