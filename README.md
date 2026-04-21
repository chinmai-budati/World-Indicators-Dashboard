# Live API Data Integration: Real-Time World Indicators Dashboard

An automated Python ETL pipeline that extracts and transforms live socio-economic data directly from the World Bank API. It features a dynamic Power BI dashboard to analyze and visualize global trends in GDP, health, and poverty in real time.

### 1. Project Overview
An automated Python ETL pipeline that extracts and transforms live socio-economic data directly from the World Bank API. This project connects the processed data to a dynamic Power BI dashboard, enabling stakeholders to monitor and visualize global trends in health, economics, and poverty in real time without manual data wrangling.

### 2. Purpose
In the real world, policymakers, NGOs, and business analysts need up-to-date global metrics to allocate resources and make data-driven decisions. The purpose of this project is to replace static, manually downloaded datasets with a live, automated tracking system. It allows non-technical users to explore complex global trends—like wealth inequality and future readiness—through an intuitive, click-based visual interface.

### 3. Tech Stack
The ETL pipeline and dashboard were built using the following tools and technologies:
* **Python (`requests`, `pandas`):** Used to script the automated fetching of paginated JSON data from the API, clean the data, merge categories, and output structured DataFrames.
* **Power BI:** The visualization tool connected directly to the Python script output, ensuring the dashboard refreshes automatically whenever new data is available.
* **World Bank Public API:** The dynamic backend data source providing verified global metrics.

### 4. Data Source
The project pulls live data from the World Bank API across several multi-dimensional categories, focusing on specific indicators:
* **Economic Data:** country_id, country_value,	indicator_name,	year,	value,	region,	incomeLevel,	lendingType, longitude,	latitude.
* **Health Data:** country_id,	country_value,	indicator_name,	year,	value,	region,	incomeLevel,	lendingType,	longitude,	latitude.
* **Poverty Data:** country_id,	country_value,	indicator_name,	year,	value,	region,	incomeLevel,	lendingType,	longitude,	latitude.
* **Labour Market Data:** country_id,	country_value,	indicator_name,	year,	value,	region,	incomeLevel,	lendingType,	longitude,	latitude.
* **Environment Data:** country_id,	country_value,	indicator_name,	year,	value,	region,	incomeLevel,	lendingType,	longitude,	latitude.
* **Technology Data:** country_id,	country_value,	indicator_name,	year,	value,	region,	incomeLevel,	lendingType,	longitude,	latitude.
* **Trade Data:** country_id,	country_value,	indicator_name,	year,	value,	region,	incomeLevel,	lendingType,	longitude,	latitude.

### 5. Features

#### Business Problem
Global development data is vast and constantly updating. Relying on manual CSV downloads creates bottlenecks and leads to analysis based on outdated information. Analysts struggle to quickly identify correlations (e.g., health spending vs. life expectancy) or spot regions requiring urgent intervention because too much time is spent prepping the data.

#### Goal of the Project
* **Automated Data Freshness:** Eliminate manual steps by establishing a live Python-to-Power BI connection that guarantees the data is always current.
* **Actionable Insights:** Build targeted visual modules that answer specific macroeconomic questions regarding poverty reduction, economic growth, and technological adoption.

#### Walkthrough of Key Modules
* **Overview:** Provides a high-level baseline of average economic and development metrics across different countries and regions.
* **Engines of Growth:** Analyzes individual economic well-being through GDP and global trade values.
* **Global Wealth & Inequality:** Pinpoints the top 10 countries succeeding in poverty reduction, alongside the bottom 10 that require urgent development interventions.
* **Future Readiness:** Explores technology adoption rates across different economic brackets to gauge digital advancement.

### 6. Business Impact & Insights
* **Operational Efficiency:** Drastically reduces reporting time by fully automating the data extraction, transformation, and loading (ETL) process.
* **Strategic Health Interventions:** Analyzes trend lines between government health expenditure and life expectancy, informing whether boosting spending is an effective lever for population health.
* **Targeted Resource Allocation:** By visually isolating countries with the least progress in poverty reduction, the dashboard helps direct NGO and donor resources where they are needed most.

### 7. Dashboard Demo:

![Dashboard Preview](https://github.com/chinmai-budati/World-Indicators-Dashboard/blob/main/Overview%20Page.png)

![Dashboard Preview](https://github.com/chinmai-budati/World-Indicators-Dashboard/blob/main/Global%20Wealth%20and%20Ineuqality%20Page.png)

![Dashboard Preview](https://github.com/chinmai-budati/World-Indicators-Dashboard/blob/main/Engines%20of%20Growth%20Page.png)

![Dashboard Preview](https://github.com/chinmai-budati/World-Indicators-Dashboard/blob/main/FutureReadiness%20Page.png)
