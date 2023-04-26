# **Global Suicide Trends & Analysis**   

### 1. Introduction: About Dataset  


#### Content 
This compiled dataset pulled from four other datasets linked by time and place, and was built to find signals correlated to increased suicide rates among different cohorts globally, across the socio-economic spectrum.

#### References  
United Nations Development Program. (2018). Human development index (HDI). Retrieved from http://hdr.undp.org/en/indicators/137506
World Bank. (2018). World development indicators: GDP (current US$) by country:1985 to 2016. Retrieved from http://databank.worldbank.org/data/source/world-development-indicators#
[Szamil]. (2017). Suicide in the Twenty-First Century [dataset]. Retrieved from https://www.kaggle.com/szamil/suicide-in-the-twenty-first-century/notebook
World Health Organization. (2018). Suicide prevention. Retrieved from http://www.who.int/mental_health/suicide-prevention/en/
  
#### Inspiration  
Suicide Prevention.

  

### 2. Import and Clean  
***Data Cleaning Change Log***  
  
* Changed column names for ease of reference (gdp_per_capita, gdp_for_year).  
* 2016 data was removed due to missing data. Few countries had any and those that did often had data missing.  
* HDI was removed due to missing data for some years and countries.  
* Removed country-year column due to duplication.  
* Removed suicides/ 100k. A more accurate calculation will be done.  
* Generation variable is not consistent.  
* Continent was added to the dataset using the `countrycode` package.  


### **Global Analysis**
![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/01-%20Global%20Suicides%20trend.png)

***Insights***  

* Upward trend between **1991** to **1995**  
* Peak suicide rate was **15.3** deaths per 100k in **1995**  
* Decreased steadily, to **11.5** per 100k in **2015** (**~25% decrease**)  


### **By Continent**
![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/02-%20Continent%20and%20Year%20trend.png)  

***Insights***  

* European rate highest overall, but has steadily **decreased by 40% since 1995**  
* The **European rate for 2015 similar to Asia & Oceania**  
* The trendline for Africa is due to poor data quality - just 3 countries have provided data  
* **Oceania & Americas are trending upwards which is concerning**  
  
  
### **By Sex**
![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/03-%20Sex%20and%20Year%20trend.png)  

***Insights***  

* Globally, the rate of suicide for men has been **~3.5x higher for men**  
* Both **male & female suicide rates peaked in 1995** and has been declining since  
* This ratio of 3.5 : 1 (male : female) has remained relatively constant since the mid 90s  


![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/04%20-%20Gender%20Disparity%20by%20Continent.png)  

***Insights***   

* European men were at the highest between 1985 - 2015 at almost 30 suicides per 100k  
* The Americas had the lowest cases of men suicides(excluding Africa due to missing data countries) with a litle over the global avergae of 13.1 per 100k  
* Europe’s rate was at 2.3x higher than global average   


### **By Age**
![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/05-%20Trend%20by%20age%20and%20Year.png)  

***Insights***  

* Globally, suicide increases with age  
* Since 1995, suicide rate for everyone aged >= 15 has been linearly decreasing  
* The suicide rate of those aged 75+ has dropped by more than 50% since 1990  
* Suicide rate in the ‘5-14’ category remains roughly static and small (< 1 per 100k per year)  


![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/06-%20Age%20Disparity%20by%20Continent.png)  

***Insights***  

* For the Americas, Asia & Europe (which make up most of the dataset), suicide rate increases with age  
* Oceania & Africa’s rates are highest for those aged 25 - 34  

### **By Country**

![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/07-%20Global%20suicides%20by%20country.png)  

***Insights***  

* Lithuania’s rate has been highest by a large margin: > 41 suicides per 100k, per year  
* Large over representation of European countries with high rates, few with low rates  

Below is a geographical heat map of the suicide rates between the timeframe of this analysis - note the lack of data for Africa and Asia, and bear in mind that 7 countries have been removed due to insufficient data.

![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/08-%20Country%20Heat%20map.png)

### **Corellation**  
![](https://github.com/John-okoye/Suicides-Rate/blob/main/Visualizations/09-%20Coreelation.png)


### **Key Insights**

* Suicide rates are decreasing globally after a spike in 1995.  
* On average, suicide rate increases with age.  
* There is a weak positive relationship between a countries GDP (per capita) and suicide rate.  
* There is an overrepresentation of men in suicide deaths at every level of analysis (globally, at a continent and country level). Globally, the male rate is at 3.5x higher.  


