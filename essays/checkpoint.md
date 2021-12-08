---
layout: essay
type: essay
title: Check Point for Assignment 3
# All dates must be YYYY-MM-DD format!
date: 2021-12-07
labels:
  - Information Technology
  - MIS
  - Management Information Systems
---


#### Shopping Cart Design

The shopping cart will be a separate page that the user can access without logging in. The button to access the shopping cart will be available on the products display page and sign-in page. As the user shops for items and adds items to their cart, the server will also add them to their session data. Whether or not a user has things in their cart, the server will add their username and email to the session data if they sign in. When the user has no items in their cart but chooses to access the cart, they will be alerted that there are no items on their shopping cart and be redirected to the products display. The user will also have the ability to add or remove items from their cart. Product inventory will not be updated until the user executes a final purchase from the cart. 

#### Data Format of Shopping Cart

When a user adds items to their cart, the product type of the items will be added to the session data as an object key. The value for each product type key will be the quantities for each product in an array format. For example, if a user adds products from multiple product types, this will be the format of item data in the session data: 
```javascript
cart data:  { Meats: [ 4, 0, 12 ], Vegetables: [ 6, 4, 1 ] }
```

#### Prevent User Access without Logging In 

Before accessing the invoice, the server will check to see if the user's username exists within the session data. The user's username is only added to the session data when logged in successfully. The server will use the same data to personalize the invoice and shopping cart. Cookies, if unencrypted, can be accessed and modified and allow the user to pose as another user. To prevent this, we encrypt the session ID with a secret. 

#### UI Personalization

When a user logs in or registers, the server will add the username and email information to the session data. This session data can be sent to the client, and when the window opens and loads, it will check for the existence of a username in the session data and load the data onto the page if it exists. 

#### Approach to Assignment 3

Assignment 3 presents a set of tasks that will require modification of current code and even removal of some code. The most difficult aspect of Assignment 3 is the ability for the user to freely roam the site (excluding the invoice page unless signed in). The user can sign in first, add items to the cart, and then checkout. Or the user can add items to the cart, sign in, then checkout. The user can also add additional items to the cart after signing in and viewing the cart. There are many paths that the user can take. My approach to his assignment will deal with each path possibility and website function one by one. When I began to write code for Assignment 3, I felt overwhelmed by the extensive and robust features that needed to be implemented into the website. After speaking with professor Port and a classmate, I recognized that the most efficient way to tackle Assignment 3 was to complete each task individually instead of implementing all functions at one time. 

#### Click [here](https://www.youtube.com/watch?v=GW1We2Lx-04) to access screencast of Assignment 3 website architecture explanation.
