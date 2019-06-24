# X_Education_Lead_Scoring

 # Business Overview
 X Education, an education company, sells online courses to industry professionals. Professionals who are interested in the courses land on their website and browse for courses. 

 # Objective
To identify hot leads (potential buyer) so sales team can focus better and increase productivity

 Analysis to be performed on leads dataset containing approx. 9000 data points
 
# Analysis Approach
Following high level approach to be used for performing the Lead Scoring analysis:
Step1: Load, Analyse, clean and impute the data.
Step2: Check correlation between continuous variables and remove unwanted attributes
Step3: Perform visualization univariate/bivariate/multivariate and create new attributes if needed (created ‘Oversees’ attribute as the conversion rate is high)
Step4: Create dummy variables for: Lead Origin, Lead Source, Last Activity, Last Notable Activity and deleted repeated variables
Step5: Check Outliers and retain data between 0.5 and 0.95 percentile
Step6: Perform feature standardization for the continuous variables and calculate initial conversion rate
Step7:  Split data into train/test and build first logistic model utilizing train data. As the number of variables are quite high, use RFE to get top 15 variables.
Step8: Optimize the model by dropping variables having p<0.5 and VIFs<5
Step9: Optimize the threshold score so the lead conversion ratio is at 80% as requested by CEO
Step10: Use this model to predict the scores on test data and compare the result with train data
