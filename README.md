# Ebay-Used-Car-Sales-Analysis-Onyx-Data-Challenge-Mar-24
## Created & Analyzed by Saddam Ansari @Aspirirng Data Analyst [Linkedin](https://www.linkedin.com/in/saddam-ansari-dataanalyst/)
### Live Dashboard at Novypro [Live_link_Novypro](https://www.novypro.com/project/ebay-used-car-analysis--onyx-data-challenge-by--saddam-ansari)

## Objective:
The objective of the **Onyx Data Challenge** in March was to analyze the ****eBay used car sales dataset**** from **Germany** spanning from **1960 to 2020**. The aim was to derive insightful insights that would benefit stakeholders. 

By meticulously examining the data, the challenge sought to answer key questions such as the most purchased car brands, the states with the highest car purchases, and the optimal months for buying cars.

## Dataset Overview:

The dataset provided for this project consisted of used car sales data from various states in **Germany** spanning the years 1960 to 2020. It comprised **371,000 rows**, each containing a multitude of attributes related to the vehicles and their transactions.

#### Key Attributes Included:

| Column name | Description |
|--|--|
|Car Name: |vehicle name.|
|Seller: |Information about the entity selling the car (e.g., private seller, comercial).|
|Offer Type: |Type of offer (e.g., offer,request).|
|Price: |The listed price of the car.|
|ABTest: |Indicates whether the listing was included in an A/B test for different site designs.|
|Vehicle Type: |Categorization of the vehicle (e.g., sedan, SUV, coupe----).|
|Year of Registration: |The year the car was first registered.|
|Month of Registration: |The month the car was registered.|
|Gearbox: |Type of transmission (e.g., manual, automatic).|
|Model: |Specific model of the car.|
|Kilometer: |The distance the car has been driven (in kilometers).|
|Fuel Type: |Type of fuel used by the vehicle (e.g., petrol, diesel----).|
|Brand: |The brand or manufacturer of the car.|
|Repaired or Not:| Indicates whether the car has undergone repairs.|
|Postal Code: |The postal code of the location associated with the listing.|
|Latitude:| Geographic coordinate representing the north-south position.|
|Longitude: |Geographic coordinate representing the east-west position.|

## Data Preparation or Cleaning Step-

During the data preparation phase for this project, it was observed that the dataset contained several blank or null values in character-type data fields. 

 * These missing values were replaced with **'Undefined'** to ensure consistency and completeness in the dataset.

 * Furthermore, the **'year of registration'** field contained numerous inaccurate entries such as 1500, 1700, 1100, and 1000, which were clearly erroneous. Entries predating **1960** were replaced with the year 1960, while entries exceeding **2019 **were replaced with the year **2020**, ensuring more realistic and accurate data.

 * Similarly, in the 'month of registration' field, it was expected that values would range from 1 to 12 to represent the twelve months of the year. However, approximately 37669 rows contained the value '0'. These entries were replaced with '1', corresponding to January, to align with the expected scale of 1-12 for the months.

#### How I calculate AVG Years of car Old?
For calculating the average age of cars, I used a field named "New Year of Registration" and extracted the year from it by subtracting it from 01/01/2020. This allowed me to determine the age of each car accurately.

#

## Dashboard Overview

The Power BI dashboard for this project is structured into three distinct pages to effectively address the project's requirements. Each page serves a specific purpose, with the first page focusing on addressing all the required and requested questions, while the second and third pages delve into optional but important analyses.

#

# Page One: Overview/Home

Page One of the dashboard provides a comprehensive overview of essential metrics and insights derived from the eBay used car sales dataset for Germany. Key performance indicators (KPIs) and visualizations offer valuable insights into various aspects of the dataset.

![mm](https://github.com/user-saddam123/Ebay-Used-Car-Sales-Analysis-Onyx-Data-Challenge-Mar-24/assets/123800896/66f2405f-ad46-4970-ae8a-7a11a8132631)


### Key Performance Indicators (KPIs):
 * Total Cars Sold: 371.40k
 * Average Car Price: €17.30k
 * Average Car Age: 16.63 years
 * Total Brands: 40
 * Vehicle Types: 9

### Car Sales by State: 

The visualization on this page presents a map view depicting the distribution of car sales across different states in Germany. The size of the bubbles on the map corresponds to the number of cars sold in each state.

##### Insight: 
Based on insights derived from the visualization, it is evident that **North Rhine-Westphalia (Nordrhein-Westfalen)** had the **highest number of car sales, with 85k units sold** throughout the dataset's duration. This observation highlights the significant market activity in this particular region.

### Sales by Seller and Offer Type:
two donut charts provide insights into car sales categorized by seller type and offer type.

#### Sales by Seller Type:
The donut chart representing sales by seller type reveals that:

 * Only 3 cars were sold by commercial sellers, indicating minimal commercial activity in the dataset. The vast majority of sales were conducted by private sellers.
 * Private sellers accounted for the majority of car sales, underscoring their prominent role in the used car market.

#### Sales by Offer Type:
The donut chart illustrating sales by offer type demonstrates that:

 * Merely 12 car sales resulted from sales requests, indicating a relatively low volume of transactions initiated by buyers' requests.
 * Conversely, the overwhelming majority of sales were initiated through other types of offers, highlighting the prevalence of fixed-price listings or auctions as the primary means of selling cars in the dataset.


### Sales by Gearbox Type:
The stacked bar chart showcases the distribution of car sales based on gearbox type:

 * Approximately 73% of the total car sales were associated with manual gearbox, indicating a prevalent preference for manual transmission among buyers.
 * Sales with automatic gearbox accounted for around 20% of the total, highlighting a significant but relatively lesser proportion compared to manual transmissions.
 * Approximately 6% of car sales were attributed to undefined gearbox types, suggesting a smaller segment of the market.

### Sales by ABTest:
The stacked bar chart illustrates the breakdown of car sales by ABTest type:

 * About 8.16% of car sales were attributed to the control test group, indicating a relatively smaller proportion of sales from this segment.
 * Notably, a substantial portion of car sales, accounting for approximately 51.84% of the total, originated from the ABTest group, indicating the significant impact of ABTest on sales.

### Car Sales by Damage Repaired or Not:
The stacked bar chart presents car sales categorized by whether damage was repaired or not:

 * Around 70% of car sales involved vehicles that were sold without any damage repaired, indicating a prevalent preference for cars in their original condition.
 * The remaining portion of sales, approximately 30%, consisted of cars that underwent some form of damage repair before being sold.

### Car Sold by Year & Month:
The visualization presents the number of cars sold each year, allowing for a comprehensive analysis of sales trends over time. Users can drill down into monthly sales data for further insights, or choose to view only the month-wise sales by clicking the "By Month Wise" button.

### Year-wise Sales:
 * In 1999, a total of 23k units were sold, indicating significant sales activity during that year.
 * The year 2020 witnessed a surge in sales, with 25k units sold, marking it as one of the peak sales years in the dataset.
 * Similarly, in 2005, car sales amounted to 22k units, reflecting another notable year for sales volume.

### Sales by Month:
Users can explore the monthly distribution of car sales to identify peak periods of sales activity.

### March and June:
 * March emerged as the month with the highest car sales, with approximately 36k units sold, indicating heightened purchasing activity during that period.
 * June closely followed, with around 33k units sold, suggesting another peak month for car sales.

#

### Sales by Brand:
The visualization provides insights into car sales categorized by brand, allowing stakeholders to understand the market share and popularity of different car manufacturers over the entire period.

### Top Selling Brands:
 * Volkswagen emerged as the leading brand in terms of sales, with a total of 80k units sold, representing approximately 21.43% of the total sales volume.
 * BMW secured the second position, with 40k units sold, accounting for 10% of the total sales.
 * Opel also achieved significant sales, matching BMW with 40k units sold, constituting another 10% of the total sales volume.

#### Analysis:
 * The top three car brands, namely Volkswagen, BMW, and Opel, collectively accounted for 40% of the total sales volume.
 * This suggests that a substantial portion of the market is dominated by these leading brands, underscoring their popularity and consumer preference.

#

### Car Sales by Vehicle Type:
The visualization presents car sales categorized by vehicle type, offering insights into the popularity and distribution of different vehicle categories over the entire dataset period.

### Top Selling Vehicle Type:
 * Limousine emerged as the most popular vehicle type, with a total of 96k units sold throughout the dataset period.
 * This accounts for a significant portion of the total sales volume, constituting approximately 25% of all car sales.

#

# Page Two: Insight / Optional

Page 2 of the dashboard offers optional but insightful analyses that provide valuable insights into various aspects of the used car market.

![mm2](https://github.com/user-saddam123/Ebay-Used-Car-Sales-Analysis-Onyx-Data-Challenge-Mar-24/assets/123800896/94817e13-cce2-4683-90c6-a59f69f4140c)

### 1. Car Sold by Fuel Type:
 * Clustered bar chart showcasing the distribution of car sales by fuel type.

 * **Insights:** Benzine fuel type vehicles recorded the highest sales, with 224k cars sold, representing 60% of the total car sales.

### 2. Top 10 Models by Number of Cars Sold:
 * Clustered column chart displaying the top 10 models based on the number of cars sold.

 * **Insights**: The Golf model recorded the highest sales at 30k units, while the Discover Sport, Series 1, and Series 3 models had the lowest sales.

### 3. KPIs:

* KPI card indicating the total number of cars with a price of 0 and the percentage of the total.

 * **Insights:** 10.78k cars were sold at a price of 0, accounting for 2.90% of the total sales.

### 4. Table: Brand-wise Sales of Cars with Price 0:
 * Table presenting brand-wise total car sales with a price of 0 and the percentage of the total.

 * **Insights:** Volkswagen had the highest number of cars sold with a price of 0, totaling 2601 units, representing 0.70% of the total.

### Additional Insights:
Clustered bar charts illustrating how fuel type, vehicle type, and brand affect the average price of cars.

 * **Fuel Type Affecting Price:** The average price of cars with 'andere' fuel type is the highest at €10,327,672, while CNG fuel type has the lowest average price at €4669.

 * **Vehicle Type Affecting Price:** 'Andere' vehicle type has the highest average price at €676,727, whereas Kleinwagen has the lowest average price at €5694.

 * **Brand Affecting Price:** 'Sonstige_Autos' brand has the highest average price at €615,956, while Daewoo brand has the lowest average price at €1017.

#

# Page Three: Tabular detailed View / Optional

![asdrf](https://github.com/user-saddam123/Ebay-Used-Car-Sales-Analysis-Onyx-Data-Challenge-Mar-24/assets/123800896/6b44aa01-f036-47bc-bc01-5921bb779c50)

 * Page 3 offers an optional tabular view where users can explore detailed insights based on their selections using various filters. This view provides a comprehensive display of insights in a structured table format, facilitating a detailed analysis of the dataset.

 * Users can utilize filters to tailor the data view according to their specific criteria, enabling them to delve deeper into the dataset and extract valuable information as per their requirements.

#











#


