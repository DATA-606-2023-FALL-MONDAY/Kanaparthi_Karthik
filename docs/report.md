# Medical Insurance Price Prediction
## Title and Author
- Project Title: Medical Insurance Price Prediction
- Prepared for UMBC Data Science Master Degree Capstone under the guidance of Dr Chaojie (Jay) Wang
- Author Name: Karthik Kanaparthi
- Fall 2023 Semester
- [GitHub](https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik)
- [LinkedIn](https://www.linkedin.com/in/kanaparthi-j-s-karthik-09b244148/)
- [PowerPoint Presentation](https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/docs/FINAL_PPT.pdf)
- [Youtube Video](https://youtu.be/wKV9AULQpn4)

## Background
#### What is this project about?
Machine learning (ML) is a technique used to predict medical insurance prices. ML algorithms examine large datasets to forecast health insurance premiums. These algorithms look for patterns and correlations by considering different variables such as age, gender, smoking status, and lifestyle. This data-driven strategy improves healthcare industry efficiency by assisting insurance companies in more precisely determining premiums and customizing policies to meet the needs of each individual.

In this case, the application of ML signifies a move toward more individualized insurance pricing. This method offers a more nuanced and fair way to determine insurance costs using sophisticated analytics and complex datasets. This could result in more equitable pricing strategies and improved risk management for insurance providers.
#### Why does Medical Insurance matter?
Medical insurance is essential because it protects people from exorbitant medical care expenses. It considerably lessens the financial burden on individuals by paying for a variety of costs, including hospital stays, therapies, and prescription drugs. This protection is crucial because it guarantees access to necessary medical treatments without the burden of prohibitive costs, particularly in emergencies or for chronic conditions requiring ongoing care.

Medical insurance also promotes preventative care, which results in an earlier diagnosis and course of treatment for health problems. By lowering costs and increasing accessibility to healthcare, it improves general public health. Financial stability is another benefit of insurance, as it shields people from unforeseen medical costs that could cause serious financial difficulties. This component of health insurance is especially important in nations where the cost of healthcare is high.
#### Research Questions
The primary research questions for Medical Insurance Price Prediction are as follows:
1. How can health-related and demographic data be used by machine learning algorithms to accurately forecast medical insurance costs?
2. What are the main determinants of medical insurance premium costs, and how do these determinants interact?
3. To what extent can machine learning models predict an individual's future healthcare costs based on their lifestyle choices and current health status?
4. How much does a person's location affect the cost of insurance, and how can machine learning account for these regional variations?
5. How can medical insurance policies be customized to each person's needs using machine learning models while maintaining fair pricing?

## Data
#### Data source
- **Data set:** [Kaggle](https://www.kaggle.com/datasets/noordeen/insurance-premium-prediction?datasetId=233212)
- **Data size:** 51KB
- **Data shape:** 1388(rows) x 7(columns/features)
- ** The time frame for the dataset was from 2012-2016**
- **Data Contains the following columns:**
    - **Age:** The age of the individuals for whom insurance information is recorded is probably contained in this column. Age plays a significant role in risk assessment and insurance premiums.
    - **Sex:** This column probably indicates the gender of the people, whether they are men or women. The cost of insurance can occasionally be influenced by gender.
    - **BMI (Body Mass Index):** The values for each person's Body Mass Index are listed in this column. Insurance companies frequently use BMI, a number derived from a person's height and weight, to evaluate health risk.
    - **Children:** This column probably lists how many children or other dependents each person has. When it comes to family insurance plans, the number of dependents may be important.
    - **Smoker:** Whether the people are smokers or not is shown in this column. Smoking influences insurance rates because it increases the risk of many different health conditions.
    - **Region:** This column probably contains information about the individuals' locations or regions. Due to variables like healthcare costs and regional regulations, insurance costs can differ by region.
    - **Expenses:** The insurance costs or premiums that each person has likely paid are listed in this column. This is the sum that people pay each year for their insurance coverage.
    
- **Main target columns are Age, Expenses, and Smoker but will use all in model development**.
#### Data Info
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/Data%20Info.png" alt="Data Info and Description" width="auto" height="250">
</p>

<div align="justify">
Data shows that there are no null values and consists of different data types like int, object, and float. The data description shows you the maximum number of counts, mean, and standard deviation.

## Exploratory Data Analysis
#### EDA 1 - Pie chart on how data divides between factors
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/EDA%201.png" alt="Pie chart on how data divides between factors" width="auto" height="300">
</p>
<div align="justify">
  Pie chart shows how the data is distributed between males and females in sex, whether the individual is a smoker or not, and how the data is divided into different regions. As you can see sex and region pie charts are equally distributed when compared to the smoker pie chart which is 80:20 ratio.
</div> 


#### EDA 2 - Comparison between expenses paid and different groups
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/EDA%202.png" alt="Comparison between expenses paid and different groups " width="auto" height="400">
</p>
<div align="justify"> 
  As you can see in the first bar graph males pay slightly higher than females do. Coming to the Smoker bar graph, if the individual is a smoker then he pays way higher than the individual who isn't a smoker. The remaining bar graphs have roughly the same prices.
</div>


#### EDA 3 - Scatter splot of expenses paid vs age and BMI respectively 
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/EDA%203.png" alt="Scatter splot of expenses paid vs age and BMI respectively" width="auto" height="400">
</p>
<div align="justify">
  You can see that there is a definite distinction between the fees that smokers must pay. Additionally, we can see that premium costs increase along with an individual's advancing years 
</div>

## Model Development
#### Models Used
#### Linear regression
A basic and effective method for predictive analytics in medical insurance pricing is linear regression. Because of its simplicity, it is perfect for comprehending the direct relationships between variables and is simple to apply and interpret. This model produces rapid predictions and is especially effective with large datasets. In addition, linear regression is an important first step in the analysis of preliminary data since it provides information about the direction and strength of relationships between independent and dependent variables, which is necessary to create more intricate predictive models.
Below are the train,test accuracy and cross validation scores attached.
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/Linear_regression.png" alt="Linear Regression scores" width="auto" height="100">
</p>

#### SVM 
In domains such as medical insurance pricing, Support Vector Machines (SVM) exhibit remarkable efficacy in predictive modeling. They work well with high-dimensional data, which makes them appropriate for intricate datasets with lots of variables. SVM provides robustness in classification and regression tasks by determining the optimal border between classes of data points. This model is a flexible option for predicting insurance prices in situations where complex patterns and interactions between variables are prevalent due to its efficacy in handling non-linear data relationships through the use of kernel tricks.
Below are the train,test accuracy and cross validation scores attached.
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/SVM.png" alt="SVM scores" width="auto" height="100">
</p>

#### Random Forest Regressor
A reliable and adaptable machine learning model that works well for forecasting tasks like estimating the cost of health insurance is the Random Forest Regressor. In order to improve prediction accuracy and reduce overfitting, it builds several decision trees during training and outputs the mean prediction of each tree individually. This ensemble approach is a preferred option for situations where accuracy and model interpretability are crucial because it manages complex datasets with numerous variables and nonlinear relationships with effectiveness. Knowing which features are important is made easier by its capacity to shed light on the factors that affect insurance rates.
Below are the train,test accuracy and cross validation scores attached.
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/Random_forest.png" alt="Random Forest Regressor scores" width="auto" height="130">
</p>

#### Gradient Boost Regressor
An excellent predictive model for applications such as predicting medical insurance premiums is the Gradient Boosting Regressor. It builds trees one after the other in an attempt to fix the mistakes of the previous one, culminating in a strong aggregated model. This method works especially well with intricate datasets that are frequently used in insurance pricing because it can capture complex, non-linear relationships in data. The model is a useful tool for accurate and nuanced predictive analysis in insurance contexts because of its capacity to handle different types of data and gradually increase prediction accuracy.
Below are the train,test accuracy and cross validation scores attached.
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/Gradient.png" alt="Gradient Boost Regressor scores" width="auto" height="130">
</p>

#### XGB Regressor
The XGBoost (Extreme Gradient Boosting) Regressor is a great option for predictive modeling in fields like medical insurance pricing because it is a highly effective and scalable gradient boosting implementation. Its performance and speed, particularly when managing big and complicated datasets, are its strongest points. To effectively predict insurance costs, complex patterns in data must be captured, and XGBoost offers a reliable method for doing so. Furthermore, it provides sophisticated functions like regularization and handling missing values, which lessen the likelihood of overfitting and boost the model's ability to predict outcomes in a variety of situations.
Below are the train,test accuracy and cross validation scores attached.
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/XGB.png" alt="XGB Regressor scores" width="auto" height="130">
</p>

#### Train VS Test Split
A balanced approach to model evaluation is provided by training different models such as SVM, XGBoost, Random Forest, Gradient Boosting, and Linear Regression using an 80/20 train-test split. By doing this split, a sizable portion of the dataset is guaranteed to be used for training, enabling the models to absorb knowledge from a wide variety of data points. Concurrently, setting aside 20% of the data for testing guarantees that the models' efficacy can be precisely evaluated on unseen data, offering a realistic assessment of their predictive capacities in real-world situations such as predicting medical insurance prices. This methodology aids in finding the best model for the task at hand and supports strong model validation.

#### Packages used
- pandas
- matplotlib
- sklearn

#### Development environment
- Personal Laptop(MAC)

#### Comparison of all models
<p align="center">
  <img src="https://github.com/DATA-606-2023-FALL-MONDAY/Kanaparthi_Karthik/blob/main/pictures/Comparison.png" alt="XGB Regressor scores" width="auto" height="275">
</p>
<div align="justify"> 
  Comparing all the train,test accuracy and CV scores we can see that XGB regressor has the highest accuracy on all the parameters which tends to be consistent in future predictions.
</div>
  
## Conclusion
The potential of advanced analytics in the healthcare insurance industry is highlighted by the investigation of medical insurance price prediction using different machine learning models. To balance learning and validation, a variety of models, each with their own advantages, including SVM, XGBoost, Random Forest, Gradient Boosting, and Linear Regression, were trained on an 80/20 split. This methodology yielded valuable insights into the key variables impacting insurance expenses and illustrated the potential of machine learning to improve the precision and efficacy of insurance premium forecasts.

The study's findings highlight how machine learning is revolutionizing the cost of health insurance. These models' capacity to work with intricate, high-dimensional datasets and reveal subtle patterns highlights their importance in creating more precise, customized insurance quotes. This shows the possibility for a more sophisticated approach in the insurance business and helps insurance providers manage risk while also promising more fair and data-driven pricing for customers.

## Future Work
- To increase the precision and applicability of prediction models, a larger range of data should be incorporated, such as socioeconomic characteristics, lifestyle decisions, and regional differences in healthcare expenses.
- Investigating cutting-edge machine learning methods such as deep learning, NLP and creating real-time models that adjust insurance prices dynamically in response to changing healthcare policies and trends
- Creating a web application such that users can check how much the price can be.
  
## References
- "A Computational Intelligence Approach for Predicting Medical Insurance Cost" by Ch. Anwar ul Hassan,Jawaid Iqbal,Saddam Hussain,Hussain AlSalman,Mogeeb A. A. Mosleh,Syed Sajid Ullah  (https://www.hindawi.com/journals/mpe/2021/1162553/)
- "Health Insurance Cost Prediction using Machine Learning" by Kashish Bhatia; Shabeg Singh Gill; Navneet Kamboj; Manish Kumar; Rajesh Kumar Bhatia  (https://ieeexplore.ieee.org/document/9824201/references)
- https://www.kaggle.com/datasets/noordeen/insurance-premium-prediction?datasetId=233212
