# Natural Disasters' Impact on Housing Prices
The project looks at the historical frequency of natural disasters' impact on change in housing prices in the last decade using linear regression. The goal of the project is to find the best linear model and the features to improve the predictive capacity the highest while maintaining the interpretability value of using linear regression. 

## Data Sources per Feature
1. Zillow Housing Prices Dataset - Housing Price %
2. Columbia University Geocoded Disasters Dataset - # of Disasters
3. Open Weather Map API - Air Pollution & November Temperature
4. World Resources Institue Energy Generation Dataset - Renewable Generation Capacity
5. US Census Bureau Boundary Dataset- Census Tract Boundary SHP File
6. Open Intro Organization County Dataset- County Level Demographic Information

Read Section 3 in the pdf to learn more about how the datasets are merged together.

## Installation
You can download the datasets and the <b>Indepent Project Everything.pynb</b> folder. The folder includes the code needed to merge the datasets together for it to be ready for any model. However, you can find the code used to conduct the three separate linear regression tests, visualizations and statistical tests used to help support the testing of new models, and the follow-up tests done to check if the model meets the Gauss-Markov assumptions for a reliable interpretation of the results.

You can read the <b>DA Independent Research Project.pdf</b> document to learn more about the hypothesis, features, methods, process and the results.

## Usage
<b> Final Model Results </b><br/> 

<img width="692" alt="Screen Shot 2022-03-22 at 10 40 41 AM" src="https://user-images.githubusercontent.com/50467434/159508139-7d098984-cb8e-4637-b982-cc3f035de18f.png">
The final model shows a relatively strong negative relationship between frequency of disasters in a given county and the changes in housing prices in the last decade. There is however a quadratic relationship between the two variables; after a certain point, the higher number of historical frequency of natural disasters has a positive relationship with changes in housing prices. 

Looking at the conditioned on variables, having high PM10 particles in the center of the county (measure used to represent air pollution) implies the highest increase in housing prices; this variable is most likely an endoneous variable as there is likely another variable that's causing people to move to certain cities, consequently increasing both air pollution and housing prices at the same time. From other variables, high population density, renewable energy generation capacity, and high november tempeartures are also positively related, in varying degrees, to changes in housing prices in the last decade.

## Roadmap
Given the quadratic relationship between frequency of natural disasters and changes in housing prices in addition to the strong positive relationship between air pollution and the dependent variable, the changes in prices are likely driven by other factors. Adding new data points to see how the relationship changes would be an interesting next step. Additionally, trying out different models to predict housing prices more accurately could also be a good next step.
