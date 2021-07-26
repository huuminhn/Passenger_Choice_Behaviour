## Python: Classification and Prediction of Airlines and Airports choice.
This project served  an academic project that is prohibited to share the original dataset and codes due to privacy.  
Summary of key findings and insights will be provided.

---

### Problem and Data Description:
#### Project objective:
This project based on South Korea, specifically two international airports in Seoul Metropolitan Area:  
- **Gimpo airport**: Smaller and old, but closer to the city 
- **Incheon airport**: Larger and new hub airport, but farther from the city
<img src="Airports.png?raw=true"/>
To recognize and predict the main reasons of how passengers choosing such airports and airlines is the main aim of this project.  
Also, discuss substantive policy implications based on the quantitative analysis.  

---
#### The Dataset: 

**Data sets**: 27 variables from survey data of 488 respondents.
- Airport choice: Gimpo, Incheon.
- Airline choice: Korean Air, Asiana Air, Korean LCC, Foreign Carriers.
- Socio-demographic: age, gender, occupation, income, etc.
- Alternative-Specific : flight information, travel time, mode of transport, etc.
---
#### Exploratory Data Analysis:
 - Data Processing: Treat outliers, Missing Values, wrong-format data cells.
 - Future Engineer: Re-categorize variables  
  -Airports: Foreign Carriers vs. Korean Carriers  
  -Airlines: E.g. Occupation (regroup 12 categories into 4): Business, Government, Unemployment and Other
 - Descriptive Statistic.
 - Data Visualization.
---
#### Model Building: 
- Variable selection:   
-Using the Holdout method to split the dataset, and using Backward/Forward method for variable selections.  
-Conduct Correlation Analysis and EDA to allocate potential  independent variables.
<img src="Correlation.png?raw=true"/>

- Build a Logistic Regression Model using the above variables from selection step.
- Build a Decision Tree Model which can be demonstrated as below: 
<img src="Tree.png?raw=true"/>

---

#### Result:  
- For Airport choices: Logistic Regression has accuracy of 84%, higher than that in Decision Tree at 78%.
- For Airlines choice (regrouped as Foregin Carriers and Korean Carriers): Logistic Regression has accuracy of 71%, slightly higher than that in Decision Tree at 68%.  
- Logistic Regression Model performs more efficiency in term of accuracy and  recall rate.

