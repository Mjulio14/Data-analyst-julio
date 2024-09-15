# Data-analyst-julio

Project Description: Exploratory Data Analysis (EDA) on Vancouver Property Tax Dataset

Project Title: Understanding Property Tax Trends in Vancouver: An Exploratory Data Analysis

Objective: The primary goal of this project is to perform an exploratory data analysis (EDA) on the Vancouver Property Tax dataset. This analysis focuses on uncovering trends and patterns in property tax values across different property types and neighbourhoods. By analyzing various indicators such as land value, improvement value, neighbourhood code, and zoning classification, we aim to identify the factors influencing property tax assessments in Vancouver.

Dataset:
The Vancouver Property Tax dataset contains the following features:

- PID: Property ID, a unique identifier for each property.
- LEGAL_TYPE: Legal classification of the property (e.g., strata).
- FOLIO: A unique number for tracking property.
- LAND_COORDINATE: Coordinates related to the property’s location.
- ZONING_DISTRICT: The zoning district in which the property is located.
- ZONING_CLASSIFICATION: The classification of the property within its zoning district (e.g., Residential, Commercial).
- LOT: The lot number of the property.
- PLAN: The plan number for the property.
- BLOCK: The block number where the property is located.
- DISTRICT_LOT: The district lot number of the property.
- FROM_CIVIC_NUMBER: The starting civic number of the property’s address.
- TO_CIVIC_NUMBER: The ending civic number of the property’s address.
- STREET_NAME: The name of the street where the property is located.
- PROPERTY_POSTAL_CODE: The postal code of the property.
- NARRATIVE_LEGAL_LINE1: Legal description of the property (line 1).
- NARRATIVE_LEGAL_LINE2: Legal description of the property (line 2).
- NARRATIVE_LEGAL_LINE3: Legal description of the property (line 3).
- NARRATIVE_LEGAL_LINE4: Legal description of the property (line 4).
- NARRATIVE_LEGAL_LINE5: Legal description of the property (line 5).
- CURRENT_LAND_VALUE: The current assessed value of the land.
- CURRENT_IMPROVEMENT_VALUE: The current assessed value of the improvements (buildings) on the land.
- TAX_ASSESSMENT_YEAR: The year in which the tax assessment was made.
- PREVIOUS_LAND_VALUE: The assessed land value from the previous year.
- PREVIOUS_IMPROVEMENT_VALUE: The assessed improvement value from the previous year.
- YEAR_BUILT: The year the property was built.
- BIG_IMPROVEMENT_YEAR: The year when a significant improvement was made to the property.
- TAX_LEVY: The total tax levied on the property.
- NEIGHBOURHOOD_CODE: A code representing the neighborhood where the property is located.
- REPORT_YEAR: The year of the property report.

Methodology
Data Collection and Preparation:

1.- Load the Dataset:
The Vancouver Property Tax dataset was loaded using Python's Pandas library. This dataset consists of 29 columns, including identifiers, tax-related data, and property information.

![image](https://github.com/user-attachments/assets/f36afa58-8111-445f-9f05-d7d7c022d1a9)

2.- Initial Data Cleaning:
Initial data cleaning involved identifying and handling missing values and ensuring that all columns had the correct data types. Columns with missing values, such as TAX_LEVY and CURRENT_LAND_VALUE, were filled using the mean for numerical columns and "Unknown" for categorical columns.

![image](https://github.com/user-attachments/assets/89aec386-db1d-44aa-b4ff-767ce9402d14)

![image](https://github.com/user-attachments/assets/bbbf80b0-bee6-4c43-9f2d-f2043a46084c)

Descriptive Statistics:

Summary statistics were generated for numerical features like TAX_LEVY and CURRENT_LAND_VALUE to provide insights into the distribution, mean, and range of values.

![image](https://github.com/user-attachments/assets/ec9f6cd5-7dfe-4acd-bf6e-c453969f2a89)

![image](https://github.com/user-attachments/assets/91266af8-dd6c-4af3-bdad-c65195c44259)

Data Visualization:

1.- Histograms and Boxplots:
Objective: Analyze the distribution of continuous variables such as TAX_LEVY and CURRENT_LAND_VALUE.

Histogram for TAX_LEVY:
We use a histogram to understand the distribution of property tax levies across the dataset. This helps identify the range of taxes and detect any skewness in the data.

![image](https://github.com/user-attachments/assets/a2c79594-dc97-4dc7-83f3-1b641ce3168e)
![image](https://github.com/user-attachments/assets/ac03326d-2d7d-4e92-aa8c-d303bede8dd0)


Explanation:

The histogram shows the frequency distribution of property tax amounts. Most properties fall within the middle tax ranges, with fewer properties having very high or very low tax levies.

Boxplot for CURRENT_LAND_VALUE:

The boxplot is used to detect outliers and understand the spread of land values across the dataset.

![image](https://github.com/user-attachments/assets/fc089177-da4b-4a4c-b48b-7d7af4288081)
![image](https://github.com/user-attachments/assets/0d36b063-2773-4e87-a201-8009f5d801bb)

Explanation:

The boxplot reveals that most properties have land values clustered within a specific range, but there are a few outliers with significantly higher or lower land values.

2.-  Bar Chart for Property Class Distribution

Objective: Show the distribution of property classifications (ZONING_CLASSIFICATION) across the dataset.

![image](https://github.com/user-attachments/assets/61b14675-92ad-44a8-9ba7-d67822e4d5b1)

Explanation:

The bar chart illustrates the count of properties for each zoning classification. This gives a clear picture of whether the majority of properties fall under residential, commercial, or other classifications.

3.- Heatmap for Correlation Between Numerical Variables

Objective: Visualize the correlation between key numerical variables, such as TAX_LEVY, CURRENT_LAND_VALUE, CURRENT_IMPROVEMENT_VALUE, and others.

![image](https://github.com/user-attachments/assets/68ad1f83-e602-4091-aa33-bf7ae567f539)

The heatmap shows the correlations between various numerical columns. For example, there may be a strong correlation between CURRENT_LAND_VALUE and TAX_LEVY, indicating that properties with higher land values tend to pay higher taxes.

4.- Boxplot for Tax Distribution by Property Class

Objective: Compare property tax distributions across different property classes (ZONING_CLASSIFICATION).

![image](https://github.com/user-attachments/assets/86150905-5dd3-4592-ac0b-c12750b8d74a)

Explanation:

The boxplot shows how property taxes vary by zoning classification. For example, commercial properties might have higher tax levies compared to residential properties.

5.- Boxplot for Tax Distribution by Neighborhood Code

Objective: Analyze how property tax distribution differs across various neighbourhoods.

![image](https://github.com/user-attachments/assets/a34345f5-1c1c-40cc-8921-8eeb5213acb1)

This boxplot helps to analyze the variation in property taxes across different neighbourhoods. It highlights which neighbourhoods tend to have higher or lower taxes.

Performance Analysis:

Objective: Analyze the performance of different property types, neighborhoods, and key variables such as tax levies and land values.

1.- Performance by Property Class

This analysis compares average property taxes across different property classifications (ZONING_CLASSIFICATION) to determine which class has higher tax levies.

![image](https://github.com/user-attachments/assets/109c3025-56f0-4c6f-b204-ec66c452a8f4)

Explanation:

This analysis reveals that commercial properties tend to have higher average tax levies compared to residential properties. This can be attributed to higher land values and infrastructure in commercial zones.

2.- Performance by Neighborhood Code

This section analyzes the performance of properties by their neighborhood code (NEIGHBOURHOOD_CODE) to understand which neighborhoods contribute more to tax revenue.

![image](https://github.com/user-attachments/assets/11186ad7-e0cd-403d-9710-4fc0e28eda5a)

Explanation:

Some neighborhoods contribute significantly more in property taxes than others, likely due to higher property values or the presence of commercial infrastructure.

3.- Performance by Land Value

This section analyzes the relationship between land value (CURRENT_LAND_VALUE) and tax levies to understand how land valuation impacts property taxes.

![image](https://github.com/user-attachments/assets/93c9962d-a76a-4c95-8f3e-2cfa8dd26d2f)

Explanation:

The scatter plot reveals a positive relationship between land value and tax levy. Properties with higher land values generally pay more in taxes, which is expected as property taxes are often based on land valuation.

Insights and Findings

High-performing Property Classes:
Commercial properties consistently show higher tax levies compared to residential properties. This suggests that commercial zones contribute more to the overall tax revenue due to higher land values and improvements.

Variation Across Neighborhoods:
Neighborhoods with higher average property taxes are likely to be more affluent or have a higher density of commercial properties. This insight is critical for city planning and budget allocation, as tax revenue is a major source of public funding.

Land Value Correlation:
There is a clear and strong positive correlation between land value and tax levies. This means that properties with higher land assessments contribute more to the city's tax revenue, reinforcing the importance of accurate land valuations.

Zoning and Development Impact:
Properties in neighborhoods zoned for commercial use not only have higher land values but also generate significantly more taxes. Future zoning and development plans should consider the tax implications of land use to optimize revenue.

Conclusion

The analysis of the Vancouver Property Tax dataset provides several important insights. Commercial properties and properties in affluent neighborhoods contribute the most to property tax revenues. The strong correlation between land value and property taxes underscores the importance of maintaining accurate and updated land assessments.

The findings also indicate that certain neighborhoods contribute significantly more in taxes, which has important implications for city planning and infrastructure development. Areas with lower tax revenues may benefit from targeted investments to improve property values and, by extension, tax contributions.

Overall, the analysis highlights the importance of property valuation in determining tax revenue and suggests that efforts to improve land value assessments could lead to more equitable and efficient tax systems.

Tools and Techniques
Python:

Pandas: Used for data manipulation, cleaning, and analysis. It allowed easy handling of missing values, grouping, and summarizing data for visualization.
NumPy: Used for numerical operations, including filling missing values with statistical methods.
Matplotlib: This library was used to create histograms, scatter plots, and bar charts for visualizing various relationships in the dataset.
Seaborn: Used for generating more sophisticated visualizations like heatmaps and boxplots to uncover trends and correlations in the data.
Jupyter Notebook:
This tool was used to perform the analysis interactively. It enabled easy documentation of the steps involved in data cleaning, exploration, and visualization.
