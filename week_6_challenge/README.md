![6](https://github.com/olubadero/Danny_Mas_8-week_SQL_Challenge/assets/111298078/80f4c5a2-da59-436b-ace5-0029966c1291)

# Introduction
Clique Bait is not like your regular online seafood store - the founder and CEO Danny, was also a part of a digital data analytics team and wanted to expand his knowledge into the seafood industry!

In this case study - you are required to support Danny’s vision and analyse his dataset and come up with creative solutions to calculate funnel fallout rates for the Clique Bait online store.

## Case Study Questions

### 1. Enterprise Relationship Diagram
Using the following DDL schema details to create an ERD for all the Clique Bait datasets.

Click [here](https://www.db-fiddle.com/f/jmnwogTsUE8hGqkZv9H7E8/17) to access the DB Diagram tool to create the ERD.


### 2. [Digital Analysis](https://github.com/olubadero/Danny_Mas_8-week_SQL_Challenge/blob/main/week_6_challenge/Digital%20Analysis.md)
Using the available datasets - answer the following questions using a single query for each one:

- How many users are there?
- How many cookies does each user have on average?
- What is the unique number of visits by all users per month?
- What is the number of events for each event type?
- What is the percentage of visits which have a purchase event?
- What is the percentage of visits which view the checkout page but do not have a purchase event?
- What are the top 3 pages by number of views?
- What is the number of views and cart adds for each product category?
- What are the top 3 products by purchases?

  
### 3. [Product Funnel Analysis](https://github.com/olubadero/Danny_Mas_8-week_SQL_Challenge/blob/main/week_6_challenge/Product%20Funnel%20Analysis.md)
Using a single SQL query - create a new output table which has the following details:

- How many times was each product viewed?
- How many times was each product added to cart?
- How many times was each product added to a cart but not purchased (abandoned)?
- How many times was each product purchased?
Additionally, create another table which further aggregates the data for the above points but this time for each product category instead of individual products.

Use your 2 new output tables - answer the following questions:

- Which product had the most views, cart adds and purchases?
- Which product was most likely to be abandoned?
- Which product had the highest view to purchase percentage?
- What is the average conversion rate from view to cart add?
- What is the average conversion rate from cart add to purchase?

### 4. [Campaigns Analysis](https://github.com/olubadero/Danny_Mas_8-week_SQL_Challenge/blob/main/week_6_challenge/Campaigns%20Analysis.md)
Generate a table that has 1 single row for every unique visit_id record and has the following columns:

- user_id
- visit_id
- visit_start_time: the earliest event_time for each visit
- page_views: count of page views for each visit
- cart_adds: count of product cart add events for each visit
- purchase: 1/0 flag if a purchase event exists for each visit
- campaign_name: map the visit to a campaign if the visit_start_time falls between the start_date and end_date
- impression: count of ad impressions for each visit
- click: count of ad clicks for each visit
- (Optional column) cart_products: a comma separated text value with products added to the cart sorted by the order they were added to the cart (hint: use the sequence_number)

Use the subsequent dataset to generate at least 5 insights for the Clique Bait team - bonus: prepare a single A4 infographic that the team can use for their management reporting sessions, be sure to emphasise the most important points from your findings.

Some ideas you might want to investigate further include:

- Identifying users who have received impressions during each campaign period and comparing each metric with other users who did not have an impression event
- Does clicking on an impression lead to higher purchase rates?
- What is the uplift in purchase rate when comparing users who click on a campaign impression versus users who do not receive an impression? What if we compare them with users who just an impression but do not click?
- What metrics can you use to quantify the success or failure of each campaign compared to eachother?

