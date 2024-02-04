# ⭐ ***Strategic Player Recruitment Analysis: Powering Real Madrid CF's Future Success*** ⭐

## A. Introduction  

###Problem Statement: 
Real Madrid CF, one of the world's premier football clubs, is strategically planning to bolster its squad following the recent departure of key players. The club's objective is to make 
three targeted signings for the striker(ST), central attacking midfielder(CAM), and left-wing(LW) positions to reinforce squad depth and sustain its competitive edge. A budget of 200 
million Euros has been allocated for these acquisitions.

###Approach:
	Prior to finalizing player acquisitions, the club aims to conduct a comprehensive analysis of player attributes and career trends using Power BI visualizations. The key areas of 
analysis include. 

	Player Performance Trends: We will delve into individual player data to identify trends related to player performance for each of the three positions—striker, CAM, and LW. This 
	analysis will reveal the age range during which players typically reach the pinnacle of their careers in these positions.

	Key Positional Attributes: We will determine the critical attributes that significantly influence player success in these roles. This analysis will help prioritize attributes such 
	as shooting accuracy, passing ability, dribbling skills, defensive capabilities, and more.

	Development Trajectories: By comparing players' current ratings with their potential ratings, we can assess their development trajectories. This evaluation will aid in identifying 
	young talents who have the potential to become top-performing players.

	Budget Optimization: We will evaluate players not only based on their skillset but also considering their market value, wage demands, and potential return on investment. This will 
	ensure that player acquisitions align with Real Madrid CF's financial constraints.

	Strategic Recruitment: Along with data-driven insights into ideal player attributes and career trends, the club will strategically recruit young talents aged 25 or younger(subject 
	ot the detailed analysis of the trends and statistics), with an overall rating of at least 70 and a potential rating of at least 80. These players are expected to make an 
	immediate impact on the team's performance while ensuring budget adherence.

	By conducting this thorough analysis of player attributes and career trends, Real Madrid CF aims to make informed and strategic recruitment decisions that not only fulfill positional 
requirements but also align with the club's long-term objectives. This data-driven approach ensures that the selected players not only meet performance criteria but also possess attributes 
that complement the team's style of play and future aspirations.

## B. About the Dataset  

The dataset has information on 100,000 orders from 2016 to 2018 made at multiple marketplaces in Brazil. The orders include details such as order status, price, payment, freight performance to customer location, product attribute, and reviews written by customers. The geolocation data is associated to Brazilian zip codes with latitude and longitude coordinates.

This is real commercial data, it has been anonymized, and references to the companies and partners in the review text have been replaced.

## C. Software Used 

1. Microsoft Excel
2. Microsoft Power BI

## D. Data Reviewing and Cleaning

The dataset has been loaded and processed in the Power Query Editor. In order to facilitate better recognition, I had to promote headers for most of the dataset since Power Query initially struggled to identify them. Additionally, I adjusted the data types for many entries. To enhance clarity and user-friendliness, I replaced technical jargon with more understandable terms, particularly in the "product_category_name_translation" file. 

## E. Data Modelling in Power BI

The tables utilized for this analysis can be linked through a star schema with one Fact Table and five dimension tables. 
However, for the sake of the project three other tables are connect as a snowflake connection to get the desired output. 

1.  ***Fact Table:*** fact_order_items

2. ***Dimension Tables:*** dim_reviews, dim_payments, dim_products, dim_sellers, dim_status

3. ***Snowflake Tables:*** dim_geolocation(connected between dim_seller, dim_customers), dim_customers(connect to dim_geolocation), dim_date(connected to dim_status) 

## ***Note:*** 
Apart from these tables, there are two more tables in the data model. One with all the measurements created for the project and one table containing product category name translations to simplify the product category names.

The Data Model is shown below: 

![alt text](https://github.com/raktimmazumdar/Data-Analysis-for-Olist-Brazilian-E-Commerce-/blob/main/ScreenShots/Power%20BI%20Data%20Model.JPG)

## F. Data Visualization/ Dashboard in Power BI: 

The dashboard created is shown below- 

## ***1. Executive Dashboard***
![alt text](https://github.com/raktimmazumdar/Data-Analysis-for-Olist-Brazilian-E-Commerce-/blob/main/ScreenShots/Executive%20Dashboard(Main%20Page).JPG)

## ***2. Customers and Orders Details(Transactions)***
![alt text](https://github.com/raktimmazumdar/Data-Analysis-for-Olist-Brazilian-E-Commerce-/blob/main/ScreenShots/Customers%20and%20Orders%20Details(Transactions).JPG)

## ***3. Map Visuals***
![alt text](https://github.com/raktimmazumdar/Data-Analysis-for-Olist-Brazilian-E-Commerce-/blob/main/ScreenShots/Map%20Visuals.JPG)

## G. Report

The findings for the project are as follows- 

1. ***Steady Growth:*** Revenue has consistently increased over three years, peaking in November 2017, but a notable decline occurred in August and September 2018, warranting further analysis.

2. ***Customer Engagement:*** Positive customer experiences are evident, with 96K unique customers and an average rating of 4.09 across categories.

3. ***Seller Network:*** A diverse network of 3,095 sellers across Brazil contributes to a wide product range.

4. ***Category Dynamics:*** "Bed Bath and Table" dominates orders, while "Health Beauty" and "Watches Gift" lead in revenue.

5. ***Regional Performance:*** São Paulo, Minas Gerais, and Paraná excel in orders and revenue, highlighting key regional strengths.

6. ***Order Patterns:*** 60.09% of orders are on weekdays, indicating weekday-focused purchasing behavior.

7. ***Customer Concentration:*** São Paulo has the most customers, followed by Rio de Janeiro and Belo Horizonte.

8. ***Payment Diversity:*** Credit cards are favored by most customers, while Boleto and Vouchers also play a significant role.

9. ***Timely Deliveries:*** 93.23% of orders are delivered on time, contributing to customer satisfaction.

10. ***Order Status:*** Most orders (97.34%) are successfully completed, addressing the remaining processing and canceled orders can enhance efficiency.


## H. Suggestions

1. ***Uncover the Dips:***  Let's dive into the reasons behind the noticeable revenue drop in August and September 2018. By understanding the triggers, we can steer clear of such dips in the future and ensure steady growth.

2. ***Nurture Categories:***  We can give some extra attention to categories that might not be shining as brightly. Through well-planned marketing efforts and engaging campaigns, we can bring them back into the spotlight and boost their performance.

3. ***Empower Reviews:***  Encouraging customers to share their experiences through reviews can have a ripple effect. Not only will this enhance credibility across categories, but it'll also build a stronger sense of trust with our customer base.

4. ***Expand Horizons:***  Exploring new regions where we're not as prominent could be an exciting step. By reaching out to untapped markets, we can broaden our reach and build a fresh customer base.

5. ***Weekend Adventure:***  We've noticed a different rhythm in weekend purchasing behavior. Let's create some weekend-specific promotions to tap into this trend and make the most of these windows of opportunity.

6. ***Seller Synergy:*** Our top-performing sellers are our champions, but we shouldn't forget the others. By offering support and collaboration, we can elevate the offerings of all our sellers, improving our overall marketplace.

7. ***Payment Ease:***  More options mean more convenience for our customers. Collaborating with additional payment gateways can make the buying process smoother and more tailored to individual preferences.

8. ***Process Precision:***  Our order processing pipeline could use some streamlining. Reducing the percentage of orders in processing status will not only expedite the process but also improve customer satisfaction.

9. ***Localize Marketing:***  Different regions have different vibes. Tailoring our marketing strategies to each region's preferences can help us create deeper connections and boost customer acquisition.

10. ***Operational Excellence:***  Keeping up our track record of on-time deliveries is crucial. By refining our inventory management and logistics, we can uphold our high standards while also optimizing costs.


## Conclusions: 

Hopefully with these findings and questions answered, I'll be able to help Olist gain better insights into their e-commerce platform and know how to optimize available opportunities for growth. Also, working  with this dataset expanded my understanding of e-commerce business metrics, enhancing my proficiency in Power BI DAX, data modeling and dashboard creation. 

Feel free to explore the merged data and analysis results for a deeper understanding of Telangana's tourism landscape.
For any questions or feedback, please contact me at raktimmazumdar11@gmail.com.


# **Best of Luck.** 👍
