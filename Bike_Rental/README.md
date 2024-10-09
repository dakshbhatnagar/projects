# 🏪 Bike Rental Shop - SQL Case Study

## 📋 Introduction
Emily is the shop owner, and she would like to gather data to help her grow the business. 


![image](https://freedo.rentals/static/media/product-slider.d4f714f5b4d90aae583e.png)


She has hired you as an SQL specialist to get the answers to her business questions, such as:

- **How many bikes does the shop own by category?**
- **What was the rental revenue for each month?**



The answers are hidden in the database, and our job is to figure out how to extract them using SQL.

This case study is taken from [LearnSQL.com](https://learnsql.com). It is part of the **"November 2023 SQL Challenge"** course.


## 🗄️ Understanding the Database
The shop’s database consists of **5 tables**:

1. `customer`
2. `bike`
3. `rental`
4. `membership_type`
5. `membership`


### 1. `customer` Table
Contains details about the customers of the bike rental shop.

| Column Name | Description                               |
|-------------|-------------------------------------------|
| `id`        | The unique ID of each customer.           |
| `name`      | The customer’s name.                      |
| `email`     | The customer’s email address.             |


### 2. `bike` Table
Holds information about the bikes owned by the rental shop.

| Column Name       | Description                                         |
|-------------------|-----------------------------------------------------|
| `id`              | The unique ID of the bike.                          |
| `model`           | The model of the bike.                              |
| `category`        | The type of bike (e.g., mountain, road, hybrid, etc.)|
| `price_per_hour`  | The rental price per hour for the bike.              |
| `price_per_day`   | The rental price per day for the bike.               |
| `status`          | The status of the bike (available, rented, out of service). |


### 3. `rental` Table
Connects customers with the bikes they have rented.

| Column Name       | Description                                          |
|-------------------|------------------------------------------------------|
| `id`              | The unique ID of the rental entry.                   |
| `customer_id`     | The ID of the customer who rented the bike.          |
| `bike_id`         | The ID of the bike rented.                           |
| `start_timestamp` | The date and time when the rental started.           |
| `duration`        | The duration of the rental in minutes.               |
| `total_paid`      | The total amount paid for the rental.                |


### 4. `membership_type` Table
Contains information about the different membership types available for purchase.

| Column Name       | Description                                     |
|-------------------|-------------------------------------------------|
| `id`              | The unique ID of the membership type.           |
| `name`            | The name of the membership type.                |
| `description`     | A description of the membership type.           |
| `price`           | The price of the membership type.               |


### 5. `membership` Table
Provides details about individual memberships purchased by customers.

| Column Name           | Description                                          |
|-----------------------|------------------------------------------------------|
| `id`                  | The unique ID of the membership.                     |
| `membership_type_id`  | The ID of the membership type purchased.             |
| `customer_id`         | The ID of the customer who purchased the membership. |
| `start_date`          | The start date of the membership.                    |
| `end_date`            | The end date of the membership.                      |
| `total_paid`          | The total amount paid for the membership.            |