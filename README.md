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

### **Oktober 2019**
#### **The best product to sell**
* New User

![image](https://user-images.githubusercontent.com/85482667/137193658-cd1cdef9-aebd-4be2-aff4-489b54470a1b.png)

* Repeat User

![image](https://user-images.githubusercontent.com/85482667/137193736-32f81e3d-5158-4921-8456-eafec7ea8508.png)

## *Summary*

* Most consumers shop at e-commerce on Wednesday. The e-commerce business team can provide a campaign to convince customers. The campaign can be intensified on Wednesday.
* Many consumers choose brand Samsung because it already has a strong and positive image for the smartphone segment. The e-commerce business team can make bundling package promos to expand the market.
* Most repeat users buy smartphone electronics products. Meanwhile product electronics audio headphones have a very large gap. The e-commerce business team can make product bundling between electronics smartphone products and electronics audio headphones to increase profits from product categories that are still low in orders.
* Most new users buy smartphone electronics products. The e-commerce business team can make promo of this product category to attract more new market users.


