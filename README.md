# Data-analyst-julio

Exploratory Data Analysis
Project Description: Exploratory Data Analysis (EDA) on Oxford Insight Dataset

Project Title: Analyzing Performance Scores Across Continents: An Exploratory Data Analysis

Objective: The primary goal of this project is to perform an exploratory data analysis (EDA) on the Oxford Insight dataset, with a focus on understanding trends and patterns in performance scores across continents. By analyzing different indicators such as government pillars, technology sectors, and GDP per capita, we aim to gain insights into what influences high performance in different regions.

Dataset: The Oxford Insight dataset contains various country performance indicators, including:

• Country: The name of each country analyzed.
• Global Ranking (2023): The country's global ranking in 2023.
• Total score (2023): The total performance score for the country in 2023.
• Government Pillar (2023): The score for the government sector in 2023.
• Technology Sector Pillar (2023): The score for the technology sector in 2023.
• Data & Infrastructure Pillar (2023): The score for data and infrastructure in 2023.
• Foreign direct investment, net inflows (% of GDP) (2023): Foreign direct investment as a percentage of GDP for 2023.
• GDP per capita (current US$) (2023): The gross domestic product per capita in current US dollars for 2023.
• Gross domestic savings (% of GDP) (2023): The gross domestic savings as a percentage of GDP for 2023.
• Gross fixed capital formation (% of GDP) (2023): The gross fixed capital formation as a percentage of GDP for 2023.
• Gross fixed capital formation (current US$) (2023): The gross fixed capital formation in current US dollars for 2023.
• Mobile cellular subscriptions (2023): The number of mobile cellular subscriptions in 2023.
• Regulatory Quality: Estimate (2023): An estimate of the quality of regulations in 2023.
• Global Position (2022): The global position of the country in 2022.
• Total score (2022): The total performance score for the country in 2022.
• Government Pillar (2022): The score for the government sector in 2022.
• Technology Sector Pillar (2022): The score for the technology sector in 2022.
• Data & Infrastructure Pillar (2022): The score for data and infrastructure in 2022.
• Foreign direct investment, net inflows (% of GDP) (2022): Foreign direct investment as a percentage of GDP for 2022.
• GDP per capita (current US$) (2022): The gross domestic product per capita in current US dollars for 2022.
• Gross domestic savings (% of GDP) (2022): The gross domestic savings as a percentage of GDP for 2022.
• Gross fixed capital formation (% of GDP) (2022): The gross fixed capital formation as a percentage of GDP for 2022.
• Gross fixed capital formation (current US$) (2022): The gross fixed capital formation in current US dollars for 2022.
• Mobile cellular subscriptions (2022): The number of mobile cellular subscriptions in 2022.
• Regulatory Quality: Estimate (2022): An estimate of the quality of regulations in 2022.
• Global Position (2021): The global position of the country in 2021.
• Overall Score (2021): The overall performance score for the country in 2021.
• Government (2021): The score for the government sector in 2021.
• Technology Sector (2021): The score for the technology sector in 2021.
• Data & Infrastructure Pillar (2021): The score for data and infrastructure in 2021.
• Foreign direct investment, net inflows (% of GDP) (2021): Foreign direct investment as a percentage of GDP for 2021.
• GDP per capita (current US$) (2021): The gross domestic product per capita in current US dollars for 2021.
• Gross domestic savings (% of GDP) (2021): The gross domestic savings as a percentage of GDP for 2021.
• Gross fixed capital formation (% of GDP) (2021): The gross fixed capital formation as a percentage of GDP for 2021.
• Gross fixed capital formation (current US$) (2021): The gross fixed capital formation in current US dollars for 2021.
• Mobile cellular subscriptions (2021): The number of mobile cellular subscriptions in 2021.
• Regulatory Quality: Estimate (2021): An estimate of the quality of regulations in 2021.

Methodology:

Data Collection and Preparation:

Load the Oxford Insight dataset using Python libraries like Pandas.

![ ](https://github.com/Mjulio14/Data-analyst-julio/blob/main/Images/Data%20Collection%20and%20Data%20Cleaning.jpg)

Perform initial data cleaning, which includes handling missing values, correcting data types, and ensuring clarity in column names

![ ](https://github.com/Mjulio14/Data-analyst-julio/blob/main/Images/Data%20Cleaning.jpg)

Descriptive Statistics:

Generate summary statistics (mean, median, mode) for numerical features like Total Scores and GDP per capita.
Count the missing values and calculate their proportion across columns to identify gaps in the data.

![ ](https://github.com/Mjulio14/Data-analyst-julio/blob/main/Images/Summary%20Statistics.jpg)

Data Visualization:

Histograms and Boxplots: Analyze the distribution of continuous variables such as government pillar scores and technology sector scores.
Bar Charts: Display performance differences across continents, focusing on overall scores and specific pillars.
Heatmaps: Visualize correlations between numerical variables like GDP, government pillar, and technology sector.

Global analysis of the data reveals variation in economic and technological development across countries. Globally, scores vary widely, with some countries achieving high levels of infrastructure, technology and regulatory quality, while others face greater challenges in these areas.

In Asia, Singapore is the leader with a total score of 81.97, excelling in all pillars, especially in governance and data infrastructure. South Korea also ranks highly with a score of 75.65. However, countries such as Malaysia, while having good overall scores, still need improvement in their technology sector. In contrast, China, although strong in data infrastructure, shows areas for improvement in its technology sector.

In South America, Brazil is one of the standout countries with a high penetration of mobile technology and a significant attraction of foreign direct investment. However, its GDP per capita is lower and needs to improve its fixed capital formation. The same is true for Argentina and Chile, which have been improving over the years.

On the African side, Ghana stands out negatively, with the lowest scores on several key indicators. This reflects an urgent need for improvement in areas of infrastructure, technology and regulatory quality. South Africa, while scoring better, still faces significant challenges in terms of economic stability and technological development.

Overall, to improve, many countries need to focus on developing their technology and data infrastructure, attracting more foreign direct investment, and improving regulatory quality to foster a more stable economic environment conducive to growth. 


![ ](https://github.com/Mjulio14/Data-analyst-julio/blob/main/Images/Distribution%20of%20Individual%20Variables.png)

Performance Analysis:

By Continent: Compare average performance scores across continents, highlighting top and low performers.
By Pillars: Investigate how key pillars like Government and Technology affect overall country performance.
By GDP per Capita: Examine how economic factors such as GDP per capita relate to overall country performance.

Through the correlation test performed on the database, we were able to find certain findings and trends



There is a high correlation between the Global Ranking with Gross Domestic Savings and GDP per capita, indicating that if emerging economies want to improve in the ranking, they must increase their savings and GDP per capita. 

As for the Oxford Insight pillars, the Government Pillar and the Technology Sector Pillar, they have a fairly high correlation with Gross Domestic Savings, this indicates that the more developed countries and positioned in the adoption of AI tend to have a higher domestic savings, as for emerging economies, to improve these pillars should start saving much more. Likewise, these two pillars have a high-moderate correlation with regulatory quality, which means that the better the legislation, the better the environment for innovation and AI deployment, the better it allows new technologies to develop and use their functions in an ethical and safe manner.

Finally the last pillar of Data & Infrastructure Pillar shows a high correlation with GDP per capita and regulatory quality, this indicates that to improve in terms of data and infrastructure there is a relationship with the GDP per capita of the country, the higher the GDP per capita the higher the infrastructure for data, in emerging economies this is extremely important because this index measures the ability to scale that have the data, if you do not ensure a solid infrastructure, new technologies such as AI may be limited.

In summary, in order to improve the adaptation of AI in emerging countries, the first priority should be to increase gross domestic savings, improve regulatory quality and increase GDP per capita.


Comparison by continent:
The chart shows that Asia and South America lead in economic and technological development, with consistently high average total scores across 2021, 2022 and 2023. This indicates robust and sustained growth in these regions, driven by countries such as Singapore, South Korea and Brazil. South America has moderate and stable scores, suggesting a medium level of development with potential for improvement, with Brazil and Argentina as the main contributors.
 
On the other hand, Africa has the lowest average scores, although it shows a slight improvement in 2022 before a small drop in 2023. This suggests that, despite some progress, the region still faces significant challenges in terms of economic and technological development. The chart highlights clear regional differences in terms of development, underscoring the need for region-specific strategies to foster sustained and balanced growth.




Insights and Findings:

When analyzing the comparative graphs between high- and low-performing countries, it is observed that high-performing countries consistently outperform low-performing countries on indicators such as the governance pillar, the technology sector, data infrastructure and GDP per capita. This suggests that these factors are crucial for economic and technological development. High-performing countries, which include regions in Asia and South America, show a clear advantage in these areas, highlighting the importance of investing in technology and infrastructure.
On the other hand, low-performing countries, predominantly in Africa, it shows an urgent need to improve these indicators to boost their development. The analysis highlights that improving the quality of governance, strengthening the technology sector, developing data infrastructure and increasing GDP per capita are essential to closing the development gap between high- and low-performing regions.

![image](https://github.com/user-attachments/assets/bb2e264c-46ef-4fa7-a565-2243a02356ed)

Conclusion:

Discuss the broader implications of the findings, such as the potential policy focus for underperforming regions or the need for further analyses, like predictive models to forecast performance scores based on various indicators.

Tools and Technologies:

Python: Pandas, NumPy, Matplotlib, Seaborn for data manipulation and visualization.
Jupyter Notebook for interactive data exploration and documentation of steps.
Optional: Tableau or Power BI for advanced visualizations and presentation.
Deliverables:

A comprehensive Jupyter Notebook documenting all steps of the analysis, with code, visualizations, and explanations of findings.
A presentation summarizing key insights and visualizations, suitable for stakeholders or peers.
