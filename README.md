# Project-1-Challenge
Looking into and Understanding Disease Risks and Causes

Title: Leading Factors of Heart Disease	
Group Members: Em Greene, Gabriel Rodriguez, Noor Zaki

In this project we look at several factors related to heart disease and evaluate their relationship to age and the significance of their relationship to heart disease. We pulled the dataset from Kaggle. It is called “Predicting Heart Disease using Clinical Variables” there are 270 patients evaluated on 13 features of heart disease. Credit for this dataset’s availability goes to Robert Hoyt, MD.

In our analysis we took out a few items as their relationship to heart disease was not explained in the dataset’s description, and we could not confidently make an analysis of these items without the additional information. These were FBS over 120, Slope of ST, and Thallium, and  we also removed the index row as that was not necessary. The data had no duplicates and no N/A values, so it was a very clean dataset.
	
    
After cleaning the data, we looked at a few of the items using summary tables of the mean, median, variance, standard deviation, and standard error of measurement for Age, Blood Pressure (BP), Cholesterol, Max HR, and ST Depression. For each of these summary tables, the group with Heart Disease present had a higher mean, with the exception of Max HR, which had a lower average value in the group with heart disease present. 
	
    
For the next block of code, we created some visualizations of the distribution of Sex, Exercise Angina, Chest Pain Type, EKG results, and Heart Disease presence and absence using pie charts so we could visualize the distribution of each of these factors. In these visualizations we found that the majority of the population of the study was male. Heart Disease was present in a little less than half of the 270 patients. EKG results were positive for atypical heart rhythm for about half of the population. About half of the population of the study experienced some sort of chest pain with exercise, with 33% experiencing severe pain, or exercise induced angina.

In the next section, we created visualizations with scatterplots and regression looking at the comparison of age and a few of the factors, to see if there was a relationship between age with Cholesterol, Max HR, BP, or ST Depression. Looking at these regression plots, we can see each had a correlation with age, although ST Depression was weakest.

Finally, we took a look at each of the factors in each group (with and without heart disease) and ran an independent t-test on the factors to see if there is a significant difference between the groups’ scores. In this analysis, we found significance at a p-value of less than 0.05 for all of the factors. The top 3 factors that are most significantly different between the groups were: “Number of Vessels fluro” which are the numbers of vessels that show in a Fluoroscopy, and this is higher in the group with Heart Disease (t-statistic: 7.98 p-value: 1.3x10^ -13) ,  Chest pain type experienced during exercise is significantly higher for the Heart Disease group (t-statistic: 7.67 p-value: 3.3x10^ -13), and Max HR is significantly lower in the group with heart disease (t-statistic: -7.39 p-value: 2.6x10^ -12). 
