# gender_inequality_project

The Gender Inequality Index (GII) provides a comprehensive measure of gender inequality across countries, capturing gender disparities in health, education, and economic opportunities. Developed by the United Nations Development Programme (UNDP), GII measures gender inequality by analyzing health, empowerment, and labor market participation indicators.

This dataset from Kaggle includes GII scores, as well as component scores for each indicator, for 195 countries, in 2021.

Project goal:
The target variable or variables under this project will be health indicators of maternal mortality and adolescent birth rate and how they depend on the GII or the proportion of women in the parliament.

The question of this EDA is to see if countries can improve their health indicators by increasing the number of women parliamentarians.

The features used in this project are social determinants of inequlity such as health (maternal mortality), education (adolescents birth rate, secondary education by gender) and political (parliametary seats) influence gender inequalities.

Risks or limitations: this dataset does not provide other information such as income or mental health issues. In addition, GII may be important for more developed countries where this index is already high.

Descriptive statistics:
The df.describe method produced mean, min and max values. For maternal mortality, the mean is 160, the minimum value of 2 was reported in Poland, Norway, Italy and Belarus and the maximum values of 1120-1150 were reported in Sierre Leone, Chad and South Sudan. For adolecent birth rate, the mean value is 44.5 and the minimum values of 1.6 to 2.3  were reported in Hong Kong, Denmark, Switzerland, South Korea and Norway. 

Correlations:
Both maternal mortality and adolescent birth rate are highly correlated with gender inequality index (more adolescent birth rate than maternal mortality), negatively correlated with female and male secondary education (more with female secondary education). Both indicators are intercorrelated which may be obvious since both are indicators of quality of health care. The scatterplots demonsrate low correlations between maternal mortality and seats in parliament and adolescent birth rate and seats in parliament. 

Histograms:
Seats in the parliament variable has normal distribution with majority of countries' female parliamentarians between 18% to 28%. The Maternal mortality and adolescent rate histograms are right scewed with higher counts of countries in the left part of the histogram with lower rates of both features. Historgram plot for education and labor by gender showed lower education coverage for girls and lower levels of labor among women than men. For example, there are countries that have lower than 10% secondary educaiton coverage among girls and no country reported similar levels of secondary education for boys. There are now countries that reported employment among male that was lower than 43%-45%.

Boxplots:
There were some outliers in each group of countries for Human Development indicators which had higher maternal morality and adolescent birth rates for their group of countries. For example, Sierra Leone, Chad and South Sudan had much higher maternal mortality in the group of countries with low human develoment index.

Decision trees:
I built three decision tree algorithms for maternal mortality, adolescent birth rate and seats in the parliament. The decision tree for maternal mortality predicts the rate of 24.9 for countries that have adolescent birth rate of less or equal to 76.7 and female secondary educaiton of more than 41.6% and then again adolencent birth rate of less than 46.65. Female seats in the parliament are not playing major role in predicting maternal mortality. Female seats in the parliament of 15% or more can predict maternal mortality but of a much higher rate of 100 per 100,000.

For adolescent birth rate, maternal mortality is a strong predictive feature. Maternal mortality of 9.5 or less predicts an adolescent birth rate of 9.5. Seats in parliament of 15% or more are predictive of adolescent birth rate but also at much higher level of 45. In feature_importances_ maternal mortality had also higher importance coefficient for adolescent birth rate than adolescent birth rate for maternal mortality. 
