# Analysis of Immigration Pattern to Canada (1980-2013)
## Introduction
This project utilizes various data visualization to analyze immigration patterns to Canada from various countries over a period of 33 years (1980-2013). The primary goal is to provide an interactive, visual representation of immigration inflows from different nations, leveraging several data science and visualization techniques such as data preprocessing, statistical analysis, and geospatial mapping.

Data Source: The data used for this analysis is derived from the United Nations’ 2015 revision on international migration flows, detailing the immigration to Canada from different countries around the world. This dataset includes immigration data from 1980 to 2013, and it also categorizes countries by region, continent, and development status (developed or developing regions).

Dataset Source:  https://www.un.org/development/desa/pd/data/international-migration-flows


Target Audience: This analysis is beneficial to policymakers, researchers, and data scientists who are interested in global migration patterns, trends in immigration to Canada, and the effectiveness of immigration policies over the decades. It also serves as an educational tool for those studying data science and geospatial analysis.

## Data Preprocessing
Author: Alex Aklson
Contributon: Jay Rajasekharan,
Ehsan M. Kermani, Slobodan Markovic], Weiqing Wang, Dr. Pooja
Objective:
Before proceeding with any analysis or visualization, data preprocessing is essential to ensure that the dataset is clean, well-structured, and ready for analysis.

Process:
Handling Missing Data: The dataset had missing values in certain columns, which were addressed through data imputation or removal, depending on the nature and significance of the missing data.
Column Renaming: To ensure clarity, some columns were renamed to more meaningful labels, for example, changing 'Continent' to 'Country Continent' to differentiate from other geographic columns.
Data Type Conversion: Data types were adjusted where necessary. For example, 'Year' columns were converted to integers, and categorical columns like 'Continent' were converted to 'category' type for efficient processing.
Normalization: Immigration data were scaled or normalized for better visualization representation, especially in choropleth maps where differences in scale can impact map interpretation.
Findings: After preprocessing, the dataset was ready for visualization and further analysis. Key insights were drawn from the processed data, such as the dominant immigration trends from specific countries and regions.

## Line Chart Analysis
Author: Alex Aklson
Contributon: Jay Rajasekharan,
Ehsan M. Kermani, Slobodan Markovic], Weiqing Wang, Dr. Pooja
Objective:
A line chart was created to visualize the overall immigration trend to Canada across the years (1980-2013). This provides an overview of how immigration numbers have evolved over time.

Process:
A line chart was plotted using the matplotlib library, with the X-axis representing years and the Y-axis representing total immigration to Canada.
Each line represented the cumulative immigration from a specific country, allowing for a comparative view of immigration trends from various source countries.
Findings:

The line chart revealed several sharp increases in immigration in the late 1980s and early 2000s, coinciding with changes in Canadian immigration policies.
Notably, countries like China, India, and the Philippines exhibited steady increases in immigration during these periods, reflecting the global migration trends influenced by socio-political changes.
## Area & Histogram Bar Plot
Author : Alex Aklson
Contributon: Jay Rajasekharan,
Ehsan M. Kermani, Slobodan Markovic], Weiqing Wang, Dr. Pooja
Objective:
The area and histogram bar plots were created to explore the distribution of immigration data across countries and regions.

Process:
An area plot was used to visualize the relative contribution of each country to the overall immigration flow to Canada.
A histogram bar plot was created to show the frequency distribution of immigration numbers, highlighting the countries with the highest and lowest immigration numbers.
Findings:

The area plot clearly showed that countries like India, China, and the Philippines dominated immigration flows, with these countries occupying the largest sections of the area.
The histogram bar plot revealed that a small number of countries contributed disproportionately to the overall immigration flow to Canada, emphasizing the importance of targeting key immigration source countries in policymaking.
## Scatter, Pie, Bubble, and Box Plots
Author : Alex Aklson
Contributon: Jay Rajasekharan,
Ehsan M. Kermani, Slobodan Markovic], Weiqing Wang, Dr. Pooja
Objective:
This set of visualizations was used to explore relationships between different variables and provide insights into the immigration data in various formats.

Process:
Scatter Plot: A scatter plot was created to analyze the relationship between the year of immigration and the total number of immigrants from various countries. This helped in understanding the correlation between time and immigration numbers.
Pie Chart: A pie chart was used to show the proportion of immigration by continent to Canada, highlighting which continents contribute most significantly to immigration flows.
Bubble Chart: A bubble chart was employed to compare countries based on the total immigration and the year of highest immigration, allowing for a dynamic view of the data.
Box Plot: A box plot was created to analyze the distribution of immigration data across countries, showing outliers and the spread of immigration numbers across different regions.
Findings:

The scatter plot confirmed that significant spikes in immigration tend to occur in certain years due to policy changes.
The pie chart revealed that Asia and Europe were the largest contributors to immigration, with Asia standing out due to high immigration from China, India, and the Philippines.
The bubble chart showed how some countries experienced an initial surge in immigration that tapered off, while others continued to grow steadily.
The box plot indicated that most countries have moderate immigration, but a few countries (such as China and India) are clear outliers with exceptionally high immigration numbers.
## Matplotlib Direct Plotting
Author : Alex Aklson
Contributon: Jay Rajasekharan,
Ehsan M. Kermani, Slobodan Markovic], Weiqing Wang, Dr. Pooja

Objective:
Matplotlib was used to directly plot bar charts, line plots, and histograms to represent the immigration data visually.

Process:
Bar charts and line plots were created to display the yearly totals and immigration trends, respectively.
Specific countries’ immigration flows were plotted to visualize their contributions to Canada’s overall immigration.
Findings:

Bar charts made it easy to compare the total immigration flows from various countries.
Line plots demonstrated how immigration surged in the 1990s and 2000s, largely driven by changes in immigration policies.
Histograms illustrated the distribution of immigration across different years, revealing that the highest immigrant numbers were in the 2000s.
## Waffle, Regression, and Word Clouds
Author : Alex Aklson
Contributon: Jay Rajasekharan,
Ehsan M. Kermani, Slobodan Markovic], Weiqing Wang, Dr. Pooja

Objective:
This section included the creation of Waffle charts, Regression analysis, and Word Clouds to provide additional insights into the dataset.

Process:
Waffle Chart: The Waffle chart visualized the proportion of immigration by country, offering a visually appealing way to compare countries.
Regression Analysis: Regression analysis was performed to predict trends in immigration based on historical data, offering insights into future immigration flows.
Word Clouds: A word cloud was generated to highlight the most frequent terms in the dataset, with a focus on the countries contributing the highest immigration numbers.
Findings:

The Waffle chart revealed that a small number of countries contributed disproportionately to immigration.
The regression model suggested a continued increase in immigration from countries like India and China, while some other regions (like Europe) showed slower growth.
The word cloud emphasized the dominance of countries like China, India, and the Philippines in the immigration data.
## Geospatial Choropleth Map
Author : Alex Aklson
Contributon: Jay Rajasekharan,
Ehsan M. Kermani, Slobodan Markovic], Weiqing Wang, Dr. Pooja

Objective:
The final geospatial visualization was the Choropleth map, which effectively showed immigration flows to Canada from different countries.

Process:
A GeoJSON file defining the geographical boundaries of countries was combined with the immigration data.
Using the Folium library, a Choropleth map was generated to visualize the immigration flows. Each country’s color was determined based on the total number of immigrants, with darker colors indicating higher immigration levels.
Findings:

Countries like China, India, and the Philippines were highlighted as the largest contributors to immigration, with dark red colors on the map.
The map visually demonstrated how immigration patterns were distributed globally, with Asia and Europe standing out as the largest contributors.
Conclusion
This project offers a comprehensive, detailed analysis of immigration to Canada over a period of 33 years. By utilizing a combination of various visualization techniques such as line charts, area plots, scatter plots, and geospatial Choropleth maps, we gained valuable insights into immigration trends and patterns. The geospatial map, in particular, provided an intuitive understanding of global immigration flows, highlighting key countries and regions.

Key Insights:
Highest Immigrations: Countries like China, India, and the Philippines showed the highest immigration flows to Canada, significantly impacting Canadian demographics.
Regional Contributions: Asia and Europe were the dominant contributors, with several countries from these continents consistently appearing in the top contributors list.
Time-Based Trends: Immigration flows to Canada have steadily increased since the 1980s, with spikes in the 1990s and 2000s due to policy shifts.
Outliers: A few countries, such as China and India, stand out as outliers with disproportionately high immigration numbers.
Acknowledgments
This project was completed as part of the IBM Data Science Professional Certificate Program and served as a hands-on exercise for learners to apply data science skills using real-world datasets.

IBM: This project benefited from the structured learning materials and resources provided by IBM’s Data Science certification program.
Author Contributions: All data preprocessing, analysis, and visualization were carried out by Alex Aklson.
Final Thoughts
This analysis not only provided insights into immigration trends to Canada but also demonstrated the power of data visualization and geospatial mapping to communicate complex data patterns. It serves as a strong foundation for anyone looking to explore the intersection of data science, geospatial analysis, and policy evaluation.

Completed by:
Qazi Fabia Hoq
As part of IBM's Data Science Professional Certificate Program

