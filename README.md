# Fleet_Data_Analysis

## Introduction: 

This report provides a comprehensive analysis of an aircraft fleet dataset, including details such as aircraft type, parent airline, operational status (Current, Future, Historic), unit cost, orders, total cost, and average age. The objective is to understand trends in fleet composition, investment, and aging patterns across airlines and aircraft models, and to highlight potential insights relevant for decision-making in fleet management and procurement planning.
This report aims to explore and analyze the dataset on HR attrition. Let’s delve into the details:

## 1.	Data Overview:

-	The dataset includes the following key features:

  •	Parent_Airline: Airline operating the aircraft.

  •	Aircraft_Type: Type/model of aircraft (e.g., B737, A320).

  •	Current, Historic, Future: Fleet count by operational status.

  •	UnitCost: Cost per aircraft in million USD.

  •	Orders: Number of aircraft ordered.

  •	 Average_Age: Mean age of aircraft in years.

  •	Total_Cost: Derived as UnitCost × Total Aircraft.

-	These variables provide an overview of the size, investment, and status of airline fleets globally.
  
2.	Data Preparation:

-	Before conducting the analysis:

•	Null values were checked using df.isnull().sum() and appropriate handling (imputation or exclusion) was performed.

•	Data types were verified and cleaned.

•	Outliers in columns like Average_Age were removed using the IQR method to avoid skewing the analysis.

3.	Exploratory Data Analysis (EDA):

-	Fleet Status Distribution:

• Current aircraft dominate the dataset with over 20,000 entries, followed by Historic (~16,000) and Future (~600).

• Indicates the dataset is heavily focused on active fleets, useful for operational planning.

-	Top Aircraft Types:

• Boeing 737 and Airbus A320 are the most common types, reflecting their widespread use in short to medium-haul routes.

• Airbus and Boeing models dominate the top 20 list, suggesting their market leadership.

-	Parent Airline Distribution:

• Lufthansa, IAG, and Air France/KLM have the largest fleet sizes.

• The dataset is skewed toward European and North American carriers, with notable presence from Asia (e.g., Air China, Qatar Airways).

-	Fleet Cost Trends:

• American Airlines has the highest total aircraft cost (~$121 billion), followed by Lufthansa and United Airlines.

• Airlines with both high fleet cost and high future orders (e.g., American, United) indicate ongoing expansion and fleet renewal.

-	Aircraft Age vs Cost:

• A negative correlation exists: newer aircraft tend to have higher unit costs, as shown by boxplots and scatter plots.

• Older aircraft (15–30 years) have significantly lower costs, aligning with market depreciation.

-	Correlation Analysis:

• Fleet size and total cost are strongly correlated (0.69).

• Orders and total cost also show moderate correlation (0.53), implying investment is often tied to planned expansions.

4.	Visualizations:

• Bar plots and countplots were used to show aircraft type and airline distributions.

• Stacked bar charts visualized aircraft types per airline.

• Boxplots captured spread and outliers in cost and age.

• Scatter plots highlighted relationships (e.g., cost vs age).

Conclusion:

This analysis of the aircraft fleet dataset reveals:

- Airbus and Boeing dominate global commercial fleets.
  
- Lufthansa and American Airlines maintain some of the largest and most expensive fleets.
  
- Current operational fleets are the main focus, with limited future order data captured.
  
- Fleet modernization is evident through the presence of newer, high-cost aircraft.
  
- Correlation findings confirm that total cost is primarily driven by fleet size and ongoing orders, while average age shows weaker influence.

These insights can assist aviation analysts, procurement teams, and airline strategists in fleet planning, investment decisions, and aging asset evaluations.

