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

#### **The best category to sell**
* New User

![image](https://user-images.githubusercontent.com/85482667/137402386-e4a9edf3-df42-4d21-9674-bdb4ba991c2f.png)

* Repeat User

![image](https://user-images.githubusercontent.com/85482667/137402431-54090791-eb09-45d7-b00a-21ce47a0184a.png)

### **Best event to predict that User most likely to buy a product**
* New User

![image](https://user-images.githubusercontent.com/85482667/137402801-dfe06c34-5c00-4a19-88d2-3a974126639f.png)

![image](https://user-images.githubusercontent.com/85482667/137402602-7ccf873a-29da-45f1-a0a5-a5f2b5baaf4c.png)

![image](https://user-images.githubusercontent.com/85482667/137402655-485d1708-67fb-463f-b31b-f2393136722d.png)

* Repeat User

![image](https://user-images.githubusercontent.com/85482667/137402987-79fd6f95-9636-4333-9adb-a21732ab89db.png)

![image](https://user-images.githubusercontent.com/85482667/137402899-8b517282-c3b2-403a-a9f5-b396292a69ac.png)

![image](https://user-images.githubusercontent.com/85482667/137402938-cd77834d-ed2b-479c-88d1-bec848b5cc82.png)

### **November 2019**
#### **The best product to sell**
* New User

![image](https://user-images.githubusercontent.com/85482667/137403161-6778046f-ca74-4630-b1ae-f3f955df755b.png)

#### **The best category to sell**
* New User

![image](https://user-images.githubusercontent.com/85482667/137403269-138cf51f-a636-4eda-a060-c9fee716944b.png)

### **Best event to predict that User most likely to buy a product**
* New User

![image](https://user-images.githubusercontent.com/85482667/137403360-ecbe84cc-8681-4b4b-bcf7-bead3f477b01.png)

![image](https://user-images.githubusercontent.com/85482667/137403468-b5fcc7be-70fc-416f-a149-4c9e75518d4b.png)

![image](https://user-images.githubusercontent.com/85482667/137403529-6ac3df02-f1a2-4de9-ae73-30a228d6a031.png)

## RFM Segmentation

![image](https://user-images.githubusercontent.com/85482667/137403851-2cc4c0b0-e20d-4ad3-b578-666b8281bde0.png)


## *Summary*

* Most consumers shop at e-commerce on Wednesday. The e-commerce business team can provide a campaign to convince customers. The campaign can be intensified on Wednesday.
* Many consumers choose brand Samsung because it already has a strong and positive image for the smartphone segment. The e-commerce business team can make bundling package promos to expand the market.
* Most repeat users buy smartphone electronics products. Meanwhile product electronics audio headphones have a very large gap. The e-commerce business team can make product bundling between electronics smartphone products and electronics audio headphones to increase profits from product categories that are still low in orders.
* Most new users buy smartphone electronics products. The e-commerce business team can make promo of this product category to attract more new market users.

## *Recommendation*
Now that we've identified our customer categories, we can decide how to approach or deal with each customer.

* Champions : Reward them. Can be early adopters of new products. Will promote your brand. Most likely to send referrals.
* Loyal Customer : Upsell higher value products. Ask for reviews.
* Potential Loyalist : Offer membership / loyalty program. Keep them engaged. Offer personalised recommendations.
* Promising : Offer coupons. Bring them back to the platform and keep them engaged. Offer personalised recommendations.
* About to Sleep : Win them back via renewals or newer products, don’t lose them to competition. Talk to them if necessary. Spend time on highest possible personalisation.
* Can't Lose Them : Provide helpful resources on the site. Send personalised emails.
* Hibernating : Make subject lines of emails very personalised. Revive their interest by a specific discount on a specific product.
* Lost : Revive interest with reach out campaign. Ignore otherwise.
