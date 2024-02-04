# ⭐ ***Strategic Player Recruitment Analysis: Powering Real Madrid CF's Future Success*** ⭐

## A. Introduction  

### Problem Statement: 
Real Madrid CF, one of the world's premier football clubs, is strategically planning to bolster its squad following the recent departure of key players. The club's objective is to make 
three targeted signings for the striker(ST), central attacking midfielder(CAM), and left-wing(LW) positions to reinforce squad depth and sustain its competitive edge. A budget of 200 
million Euros has been allocated for these acquisitions.

### Approach:
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
ot the detailed analysis of the trends and statistics), with an overall rating of at least 70 and a potential rating of at least 80. These players are expected to make an immediate impact on the team's performance while ensuring budget adherence.

By conducting this thorough analysis of player attributes and career trends, Real Madrid CF aims to make informed and strategic recruitment decisions that not only fulfill positional 
requirements but also align with the club's long-term objectives. This data-driven approach ensures that the selected players not only meet performance criteria but also possess attributes 
that complement the team's style of play and future aspirations.

## B. About the Dataset  
The dataset used for Real Madrid CF's player recruitment strategy comprises FIFA player information as of 2018. It contains details such as player names, ages, nationalities, and current club affiliations. Positional focus is emphasized, with specific attention to strikers (ST), central attacking midfielders (CAM), and left-wingers (LW). Player performance is assessed through overall and potential ratings, offering insights into current skill levels and future potential. Financial aspects are considered with data on player wages and market values, aiding in budget optimization for acquisitions. The dataset also captures player attributes specific to their positions, encompassing skills like shooting accuracy, passing ability, and defensive capabilities. 
With a total budget of 200 million Euros allocated for three targeted signings, this dataset serves as a comprehensive resource for conducting a nuanced analysis to guide informed recruitment decisions

## C. Software Used 

1. Microsoft Excel
2. Microsoft Power BI
3. Python

## D. Data Reviewing and Cleaning

The dataset has been loaded and processed in the Power Query Editor. In order to facilitate better recognition, I had to adjust the data types for many entries such as date of joining, wages and values. To enhance clarity and user-friendliness, I replaced the unknown characters with more understandable terms, particularly in the "Players_fact" file. 

## E. Data Modelling in Power BI

The tables utilized for this analysis can be linked through a star schema with one Fact Table and four dimension tables. 
However, for the sake of the project three other tables are connect as a snowflake connection to get the desired output(Radar chart Visual). 

1.  ***Fact Table:*** 'Players_fact'

2. ***Dimension Tables:*** Positions_dim, Clubs_dim, Nationality_dim, Players_Attributes_dim

3. ***Snowflake Tables:*** Players_attributes_RadarChart(connected to Players_Attributes_dim via Player_id key)

## ***Note:*** 
Apart from these tables, there are one more table in the data model containing all the measurements created for the project.

The Data Model is shown below: 

![alt text](https://github.com/raktimmazumdar/Real-Madrid-Player-Recruitment---Data-Analysis-Project/blob/master/ScreenShots/Data%20Model.JPG)

## F. Data Visualization/ Dashboard in Power BI: 

The dashboard created is shown below- 

## ***1. Home Page***
![alt text](https://github.com/raktimmazumdar/Real-Madrid-Player-Recruitment---Data-Analysis-Project/blob/master/ScreenShots/Home%20Page.JPG)

## ***2. Forwards Details***
![alt text](https://github.com/raktimmazumdar/Real-Madrid-Player-Recruitment---Data-Analysis-Project/blob/master/ScreenShots/Forward%20Page.JPG)

## ***3. Mid-fielders Details***
![alt text](https://github.com/raktimmazumdar/Real-Madrid-Player-Recruitment---Data-Analysis-Project/blob/master/ScreenShots/Midfielder%20Page.JPG)

## ***4. Deferdars Details***
![alt text](https://github.com/raktimmazumdar/Real-Madrid-Player-Recruitment---Data-Analysis-Project/blob/master/ScreenShots/Defenders%20Page.JPG)

## ***5. Radar Charts Preview*** 
![alt text](https://github.com/raktimmazumdar/Real-Madrid-Player-Recruitment---Data-Analysis-Project/blob/master/ScreenShots/Forward%20Page%20with%20Radar%20Chart.JPG)
![alt text](https://github.com/raktimmazumdar/Real-Madrid-Player-Recruitment---Data-Analysis-Project/blob/master/ScreenShots/Midfielder%20Page%20with%20Radar%20Chart.JPG)
![alt text](https://github.com/raktimmazumdar/Real-Madrid-Player-Recruitment---Data-Analysis-Project/blob/master/ScreenShots/Defenders%20Page%20with%20Radar%20Chart.JPG)


## G. Findings

Real Madrid CF's data-driven approach to player recruitment and analysis has provided valuable insights for making informed decisions to reinforce the squad in key positions. The comprehensive analysis focused on player performance trends, key positional attributes, development trajectories, budget optimization, and strategic recruitment. Here are the key conclusions derived from the findings:

### 1. Total Players and Position Breakdown:

The dataset comprises 18,207 players, with specific attention to 2,668 forwards, 5,701 defenders, and 7,813 midfielders.
Real Madrid CF aims to make strategic acquisitions within a 200 million Euro budget, targeting 33 players, including 5 forwards, 12 defenders, and 12 midfielders.

### 2. Player Age and Peak Performance:

Analysis indicates that player potential steadily increases from age 20 to 26, peaking between the age range of 30-34. This insight helps identify the prime age for recruitment.

### 3. Current Squad Age Distribution:

The current squad's average age is approximately 27 for goalkeepers, 24.20 for forwards, and 23.50 for both defenders and midfielders. This information aids in aligning new signings with the existing team dynamics.

### 4. Work Rate and Overall Ratings:

For forwards, players with low/medium and high/high work rates have the highest ratings.
Midfielders with high/high and medium/high work rates exhibit the highest overall ratings.
Defenders with high/high and high/low work rates have the highest overall ratings. This insight guides recruitment based on work rate preferences.

### 5. International Reputation and Overall Ratings:

International ratings (1-5) correlate positively with overall ratings. This suggests that players with higher overall ratings tend to have a better international reputation.

### 6. Key Influencers Visual:

Top attributes influencing forwards include finishing, positioning, shot power, ball control, and reactions, identifying players like K. Mbappe, L. Martinez, and L. Jovic as potential targets.
Key attributes for midfielders encompass ball control, reactions, short passing, dribbling, vision, and crossing, highlighting J. Sancho, M. Odegaard, and K. Havertz as suitable targets.
Defenders' key attributes include standing tackle, marking, interceptions, heading accuracy, and reactions, guiding the recruitment focus towards M. de Ligt, D. Upamecano, and Eder Militao.

### 7. Budget Allocations:

Real Madrid CF will allocate funds strategically, considering both player skillsets and financial aspects such as market value, wage demands, and potential return on investment.
In conclusion, the data analysis project equips Real Madrid CF with a data-driven recruitment strategy, ensuring acquisitions align not only with positional requirements but also with the club's long-term objectives. The GitHub project incorporates detailed findings and recommendations to guide the club in making impactful and strategic player signings.

### **The Results can be further modified as per requirements by adjusting the slicers provided in the report.**

## H. Conclusion

Hopefully with these findings and questions answered, I'll be able to help Real Madrid CF gain better insights into their players recruitment strategy and know how to optimize available opportunities for the recruitment process. Also, working  with this dataset expanded my understanding of club football hiring processes and in turn enhancing my proficiency in Power BI DAX, data modeling and dashboard creation. 

Feel free to explore the data and analysis results for a deeper understanding of Strategic Player Recruitment Analysis of Real Madrid CF. 
For any questions or feedback, please contact me at raktimmazumdar11@gmail.com.


# **Best of Luck.** 👍
