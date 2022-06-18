# Spark_User Session Analysis for Large E-commerce

This project is mainly used in Internet e-commerce enterprises, using the big data statistical analysis platform developed by Spark technology to conduct complex analysis on various user behaviors (visiting behavior, shopping behavior, advertisement click behavior, etc.) of e-commerce websites. Use the data from statistical analysis to assist PM (product managers), data analysts and managers in the company to analyze the current product situation, and to continuously improve product design based on the results of user behavior analysis, as well as adjust the company's strategy and business. Finally, the goal of using big data technology to help improve the company's performance, turnover and market share is achieved.

This project uses the three most commonly used technical frameworks in the Spark technology ecological stack, <b>Spark Core</b>, <b>Spark SQL</b> and <b>Spark Streaming</b>, to develop offline computing and real-time computing business modules. It has realized 4 business modules including 
1. user access session analysis, 
2. page conversion rate statistics, 
3. offline statistics of popular products, 
4. real-time statistics of advertising traffic
 
In the project, it focuses on the knowledge and technology of performance tuning, troubleshooting and data skew in line with actual enterprise projects. At the same time, the enterprise-level big data project development process is used to explain each business module, covering the whole process of project development, including Requirement analysis, scheme design, data design, coding implementation, testing and performance tuning, etc., fully restore the development process of real big data projects.

# modules
## user access session analysis

This module mainly conducts statistical analysis on user access sessions, including the calculation of aggregated indicators of sessions, randomly extracting sessions according to the time ratio, obtaining daily clicks, placing orders and purchasing the top 10 categories, and obtaining the top 10 clicks of the top 10 categories. session. This module allows product managers, data analysts and enterprise management to visually see specific user behaviors and statistical indicators under various conditions, so as to make adjustments to the company's product design and business development strategies. Mainly implemented using Spark Core.

## page conversion rate statistics

This module mainly calculates the conversion rate of single-step jump between key pages, involving page slicing algorithm and page flow matching algorithm. This module allows product managers, data analysts and enterprise management to see the conversion rate between key pages, so as to better optimize the design of the page layout. Mainly implemented using Spark Core.

## offline statistics of popular products

This module mainly realizes the daily statistics of the top 3 popular commodities in each region. Then use Oozie for timing scheduling of offline statistical tasks; use Zeppeline for data visualization report display. This module allows enterprise management to see the overall situation of the products sold by the company, so as to adjust the company's product-related strategies. Mainly implemented using Spark SQL.
