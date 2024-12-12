<h1>The Socioeconomic Factors Contributing to Obesity in the U.S.</h1>
<h2>Saharsh Yeruva, Alex Chan, Sidharth Menon</h2>


<h3> 1 Introduction </h3>
<h4>1.1 Background Information</h4>
The prevalence of obesity worldwide has been on an upward trajectory, with this trend particularly pronounced in the United States. This is evident in the data provided by the CDC: “From 1999–2000 through March 2017–2020, obesity prevalence in the United States increased from 30.5% to 41.9%” [Centers for Disease Control and Prevention, 2022a]. CDC data suggests that 22 states have an adult obesity prevalence at or above 35%, compared to 19 states in 2021 [Centers for Disease Control and Prevention, 2022a]. By investigating a Kaggle dataset titled “Obesity and GDP Rates from 50 States in 2014-2017”, we attempt to zoom in and evaluate the socioeconomic factors that contribute to obesity in the U.S. Obesity is
traditionally defined as a medical condition characterized by the excessive accumulation of body fat. One common metric that is usually used to evaluate a person’s body mass index, a ratio of their weight to height, with a BMI of 30 or higher generally indicating obesity. However, it is important to note that although BMI is a metric that attempts to quantify
obesity, it does not account for lean muscle mass and body composition in its calculation. [Centers for Disease Control and Prevention, 2022b]. Something else that we have tried to in1 corporate into our analysis is the presence of food deserts. Food deserts are defined as areas characterized by relatively poor access to healthy and affordable food that may contribute to social disparities in diet and diet-related health outcomes. They are important to examine due to their presence serving as an explanation of the food choices of American consumers in such areas [Centers for Disease Control and Prevention, 2009].
<br />
<br />
Although obesity in isolation may not be a cause for widespread concern, the need to investigate obesity arises from its potential to act as a trigger to other severe health-related issues.
It has been documented that obesity is strongly associated with an increased risk of conditions
such as heart disease, stroke, type 2 diabetes, joint disease, and certain cancers. The economic
burden it imposes is equally concerning, with annual medical costs in the United States reaching $149.4 billion [Rosenthal et al., 2017]. These health and financial consequences outline the
critical need to investigate obesity and to learn ways to control it when required.
<h4>1.2 Factors to Consider</h4>

To understand and address obesity effectively, it is crucial to comprehend various factors that
may contribute to its prevalence. By gaining this understanding, we can explore how socioeconomic factors and geographic location impact obesity rates in America. Building on this
comprehension, we can then examine the implications of these findings for developing tailored
public health interventions.
The existing scientific literature on obesity predominantly concentrates on individual behavioral factors such as diet and exercise, as well as broader public health impacts. However,
our research attempts to focus on the socioeconomic factors, geographic location and presence
of food deserts, and cultural influences, and how these collectively contribute to the obesity
epidemic in America. We will attempt to explore obesity prevention and treatment strategies
based on the findings of our analysis.
1. Socioeconomic Factors: Research describing the detailed role of income levels, edu2
cation, and occupation in determining obesity risks. For instance, variations in obesity
prevalence and severity may exist among different income or educational groups.
2. Geographic Variations: Obesity rates and their associated health outcomes may vary
significantly across different regions, urban vs. rural areas, or among states with different
policies and resources.
3. Intersectionality: How these factors intersect and influence each other is not comprehensively understood. For example, how does geographic location interact with socioeconomic status to influence obesity rates?
<br/>
It is crucial that we fill this gap for several reasons:
<br/>

1. Tailored Interventions: Understanding the role of these factors can lead to more targeted
and culturally sensitive interventions. This can improve the efficacy of obesity prevention
and management programs.
2. Policy Development: Insights into how socioeconomic and geographic factors influence
obesity can guide policymakers in allocating resources and designing health policies that
address specific needs of diverse populations.
3. Health Equity: Exploring these aspects contributes to addressing health disparities. Populations disproportionately affected by obesity due to socioeconomic or cultural factors
need tailored strategies for effective outcomes.
4. Comprehensive Understanding: A more nuanced understanding of obesity can enhance
the overall knowledge base, leading to innovative approaches in tackling this complex
issue.
5. Long-term Impact: Addressing these underexplored areas in research can have a lasting
impact on public health, potentially reducing the economic and health burden of obesity
on a national scale.

<h4>1.3 Preexisting Literature</h4>
The cited article, titled “Impact of Food Environments on Obesity Rates: A State-Level Analysis,” [Cerceo et al., 2023] was published in the Journal of Obesity in June 2023. The research investigates the relationship between food environments and obesity rates at the state level. The study aims to assess how the availability and accessibility of food in different environments influence obesity prevalence. Utilizing a state-level analysis, the authors explore the impact of varying food environments on population obesity rates. The findings of this research contribute valuable insights into the complex interplay between the food environment and obesity, offering
implications for public health strategies and policies at the state level. Pearson correlation coefficients have been computed to paint a preliminary picture of the relationship between sleep, exercise, sleeping, and obesity. The authors use Modifed Retail Food Environment Index (mRFEI) - the ratio of healthy food retailers compared to total food retailers in a geographic region - as a metric of comparison for covariates in their regression model. Relevant results of the
linear logistic linear regression indicate that the mRFEI difference between the variables denoting food swamps and food deserts was statistically significant (p value = 0.008) and pointed towards an increased association with obesity prevalence.
</br></br>
The article “Obesity Determinants among Malaysian Schoolchildren: What Is New?” by Ahmad et al. [Ahmad et al., 2017], published in the Proceedings of the Nutrition Society in
2017, investigates the determinants of obesity among schoolchildren in Malaysia. The study delves into novel aspects contributing to obesity in this population. The authors employ a
research approach to identify and understand new factors influencing obesity in Malaysian schoolchildren. The article contributes to the scientific discourse on obesity determinants, providing potentially valuable insights for public health interventions and policies in Malaysia. The results of the Multiple Linear Regression analysis that they used to study the impact of factors such as hereditary BMI, household information indicative of socioeconomic status, and weight at birth on the BMI of the subject in question showed that all these covariates were statistically significant with p values <0.05, with obesity being negatively associated with increased household sizes while being positively associated with all the other covariates.

<h3>2 Methods</h3>
Our data came from a dataset titled Obesity and GDP Rates From 50 States in 2014-2017. This dataset makes use of several different datasets which range from macro-sources as well
as primary-sources. Macro-sources include data from ‘DataUSA’ regarding adult obesity rates, average age, average income, and poverty rates for each state. Primary-sources include data
from both the Federal Reserve as well as the U.S. Bureau of Economic Analysis regarding Real GDP by state and state region. The dataset consists of 200 observations with 18 variables.
There are four years used in this dataset: 2014, 2015, 2016, 2017. We opted to use a linear regression model to model our dataset. Our outcome variable was Adult.Obesity ( a percent decimal between 0 and 1). The predictor variables we chose to use are Region(Great Lakes, Mideast, New England, Plains, Rocky Mountain, Southeast, Southwest, Far West), Average Income(in US Dollars), Poverty Rate (Percent decimal between 0 and 1), and Real GDP Growth (Percent decimal between 0 and 1). We chose to include “Region” because the eight distinct
regions represented in the dataset could provide insight into how regional differences could have a substantial impact on lifestyle, culture, and dietary habits. Different regions may have varying access to resources, healthcare, and education, which may influence obesity rates. We chose to include “Average.Income” because income levels can affect individuals’ access to healthier food options, opportunities for physical activity, and healthcare resources. We chose to include “Poverty.Rate” because higher poverty rates may be associated with limited access to nutritious food, healthcare, and recreational facilities, contributing to higher obesity rates. We chose to include “Real.GDP.Growth” because economic growth can influence various aspects of lifestyle, healthcare infrastructure, and societal well-being. Out of the 18 variables present in our dataset, we chose to include only the 4 variables described above because a decent number of the remaining variables were redundant due to them simply being the whole number percentage value of the chosen covariates. Some other things we took into consideration while choosing these covariates in our model were the value of R-Squared to assess the goodness of fit and the normality of residuals. The model we chose ultimately struck the best balance between these two criteria. We did not have to, nor did, transform any of the variables. While we checked for any observations with NA values to remove, there were none present, so no observations were removed.


<h3>4 Discussion</h3>
<h4>4.1 Research Question</h4>

In addressing the research question, it is essential to consider the interpretation of the coefficients obtained from the regression analysis. Notably, the intercept’s interpretation may not be meaningful in this context, as it implies all covariates being zero, which is unrealistic (e.g.,
average income, poverty rate, Real GDP Growth, and region as Far West). It’s crucial to acknowledge the potential influence of unaccounted variables, such as cultural factors and physical activity, on the obesity rate. While these variables are not present in our dataset, they may play a significant role in explaining the observed results.
</br></br>
A more detailed examination of the coefficient values reveals that the Rocky Mountain
region exhibits the lowest obesity rate. One possible explanation could be the hilly terrain,
necessitating increased daily cardio and physical activity, thus promoting overall health. Interestingly, most covariates in our study are associated with a decrease in the obesity rate, aligning with our initial assumptions. However, the poverty rate shows an unexpected relationship. One hypothesis could be that individuals in poverty may face challenges in accessing sufficient food, leading to weight loss and a decrease in obesity rates.

<h4>4.2 Linear Regression</h4>
We rigorously assessed the assumptions of linear regression to ensure the validity of our model.
One critical assumption is the normality of residuals, which is pivotal for making valid statistical inferences. We conducted a thorough examination of the residuals’ distribution and found it to be relatively normal. This observation supports the assumption that the errors are approximately normally distributed. Normality is crucial for hypothesis testing, and deviations from normality could impact the reliability of our results. Therefore, the normality of residuals is a key factor to consider when interpreting our hypothesis tests and drawing conclusions from them. Additionally, we investigated the independence between variables, another fundamental assumption of multiple linear regression. Ensuring independence is vital to prevent multicollinearity issues and maintain the integrity of our model. Our careful examination confirmed that the variables in our model exhibit the necessary independence. Moreover, the relatively high R-squared value of 0.6557 is indicative of a strong fit for our model. This statistic represents the proportion of variability in the dependent variable explained by the independent variables.
</br></br>
In summary, our model satisfies the assumptions of normality of residuals and independence between variables. These findings strengthen the reliability of our hypothesis tests and the
validity of the conclusions drawn from them.

<h4>4.3 Limitations</h4>
Our study, while contributing valuable insights, is subject to several limitations that should be considered in interpreting the results. First, the decision not to use our initial dataset means that our analysis does not provide detailed information about individual lifestyles. Important factors such as diet, culture, religion, and physical activity, which could significantly influence obesity rates, are not accounted for in our study. Recognizing these omissions is crucial for understanding the broader context of obesity determinants. Furthermore, the focus on state populations in our data may obscure variations in obesity trends at a more localized level. Obesity patterns can differ significantly within states, and our analysis might not capture these nuanced variations. Future research that delves into more localized data could provide a more comprehensive understanding of regional disparities in obesity rates. Additionally, while our analysis highlights associations between predictor variables and obesity rates, it falls short of establishing causation. Establishing causation requires a more nuanced study design, potentially involving experimental or longitudinal approaches. It’s important to acknowledge that our findings indicate correlations rather than causation. Lastly, our study lacks an examination of policy and environmental factors influencing obesity. Understanding the impact of broader contextual elements, such as government policies and environmental conditions, is crucial for developing comprehensive strategies to address the obesity epidemic.Future research efforts should explore integrating these dimensions to achieve a more comprehensive understanding of the factors involved.

<h4>4.4 Next Steps</h4>
Having addressed the question through the socioeconomic lens, it is evident that there are numerous avenues for further exploration in obesity research. One promising direction involves comparative studies on the lifestyle choices of individuals across different age groups, aiming to understand the varying impacts on obesity. This approach could provide a foundation for tailoring recommendations on an individual basis, considering age-specific factors. From a medical perspective, an intriguing area for future investigation lies in researching drugs targeting enzymes related to satiation and their correlation with obesity. Exploring the safety, efficacy, and overall impact of such drugs could offer insights into new avenues for obesity management. Understanding whether these drugs provide a viable means to mitigate obesity could potentially offer individuals greater flexibility in managing their lifestyle choices. Furthermore, delving into the effectiveness and viability of precision medicine and personalized interventions in the context of obesity management holds significant promise. Investigating the potential of individualized approaches could lead to more targeted and successful strategies for preventing and treating obesity.


<h4>References</h4>
[Ahmad et al., 2017] Ahmad, A., Zulaily, N., Shahril, M. R., Manan, S., Fadzli, S., Wafa, S., Amin, R., and
Ahmed, A. (2017). Obesity determinants among malaysian schoolchildren: What is new? Proceedings of the
Nutrition Society, 76.
</br></br>
[Centers for Disease Control and Prevention, 2009] Centers for Disease Control and Prevention (2009). A systematic review of food deserts, 1966-2007.
</br></br>
[Centers for Disease Control and Prevention, 2022a] Centers for Disease Control and Prevention (2022a). Adult
obesity facts.
</br></br>
[Centers for Disease Control and Prevention, 2022b] Centers for Disease Control and Prevention (2022b). Defining adult overweight & obesity.
</br></br>
[Cerceo et al., 2023] Cerceo, E., Sharma, E., Boguslavsky, A., and Rachoin, J.-S. (2023). Impact of food environments on obesity rates: A State-Level analysis. Journal of Obesity, 2023:5052613.
</br></br>
[Rosenthal et al., 2017] Rosenthal, R. J., Morton, J., Brethauer, S., Mattar, S., De Maria, E., Benz, J. K., Titus, J.,
and Sterrett, D. (2017). Obesity in america. Surg. Obes. Relat. Dis., 13(10):1643–1650.
