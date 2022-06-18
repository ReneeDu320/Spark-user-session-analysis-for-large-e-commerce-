# Spark 大型电商项目用户会话分析

This project is mainly used in Internet e-commerce enterprises, using the big data statistical analysis platform developed by Spark technology to conduct complex analysis on various user behaviors (visiting behavior, shopping behavior, advertisement click behavior, etc.) of e-commerce websites. Use the data from statistical analysis to assist PM (product managers), data analysts and managers in the company to analyze the current product situation, and to continuously improve product design based on the results of user behavior analysis, as well as adjust the company's strategy and business. Finally, the goal of using big data technology to help improve the company's performance, turnover and market share is achieved.

This project uses the three most commonly used technical frameworks in the Spark technology ecological stack, Spark Core, Spark SQL and Spark Streaming, to develop offline computing and real-time computing business modules. It has realized 4 business modules including user access session analysis, page single jump rate statistics, offline statistics of popular products, and real-time statistics of advertising traffic.

In the project, it focuses on the knowledge and technology of performance tuning, troubleshooting and data skew in line with actual enterprise projects. At the same time, the enterprise-level big data project development process is used to explain each business module, covering the whole process of project development, including Requirement analysis, scheme design, data design, coding implementation, testing and performance tuning, etc., fully restore the development process of real big data projects.

# 模块介绍
## 用户访问session分析

该模块主要是对用户访问session进行统计分析，包括session的聚合指标计算、按时间比例随机抽取session、获取每天点击、下单和购买排名前10的品类、并获取top10品类的点击量排名前10的session。该模块可以让产品经理、数据分析师以及企业管理层形象地看到各种条件下的具体用户行为以及统计指标，从而对公司的产品设计以及业务发展战略做出调整。主要使用Spark Core实现。

## 页面单跳转化率统计

该模块主要是计算关键页面之间的单步跳转转化率，涉及到页面切片算法以及页面流匹配算法。该模块可以让产品经理、数据分析师以及企业管理层看到各个关键页面之间的转化率，从而对网页布局，进行更好的优化设计。主要使用Spark Core实现。

## 热门商品离线统计

该模块主要实现每天统计出各个区域的top3热门商品。然后使用Oozie进行离线统计任务的定时调度；使用Zeppeline进行数据可视化的报表展示。该模块可以让企业管理层看到公司售卖的商品的整体情况，从而对公司的商品相关的战略进行调整。主要使用Spark SQL实现。

