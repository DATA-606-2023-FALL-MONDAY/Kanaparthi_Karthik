# DATA 606 CAPSTONE PROPOSAL

## Medical Insurance Price Prediction

- Prepared for UMBC Data Science master’s degree Capstone by Dr. Chaojie (Jay) Wang
- Kanaparthi J S Karthik
- [GitHub](https://github.com/kjskarthik)
- [LinkedIn](https://www.linkedin.com/in/kanaparthi-j-s-karthik-09b244148/)
- Powerpoint presentation - TBD
- Youtube Video - TBD 

## Background

The ability to predict medical insurance costs has grown significantly in importance in the contemporary healthcare environment, where data-driven decision-making is crucial. Numerous variables, including individual demographics, medical conditions, and regional healthcare costs, have an impact on medical insurance premiums. For insurance companies to effectively assess risk and maintain profitability as well as to enable customers to make educated decisions when choosing insurance plans, accurate price prediction is essential. Our goal is to create a reliable and accurate model for predicting the cost of medical insurance using Python's machine learning tools. With the help of this initiative, people will be able to navigate the complicated insurance market and get the best coverage at the most affordable prices. It also promises to streamline pricing strategies for insurance companies.

Data collection, preprocessing, model choice, training, and evaluation are the main parts of this project. We can build a robust foundation for the model by combining a variety of datasets that include different individual attributes and historical insurance data. We will develop features, develop predictive models, and meticulously evaluate their performance using Python's adaptable libraries and machine learning frameworks to deliver a cutting-edge solution for predicting the cost of health insurance. This machine learning approach, which is expected to improve insurance pricing efficiency and transparency as healthcare continues to change, will ultimately be advantageous for both consumers and providers in a healthcare ecosystem that is becoming more and more data-centric.

## Research Questions

- What are the key factors influencing medical insurance premiums?
- Which machine learning algorithms are most effective for medical insurance price prediction?
- How well does the developed model generalize to new data and unseen individuals?

## Data Source

- **Data set:** [Kaggle](https://www.kaggle.com/datasets/noordeen/insurance-premium-prediction?datasetId=233212)
- **Data size:** 51KB
- **Data shape:** 1388(rows) x 7(columns/features)
- **Data Contains the following columns:**
    - **Age:** The age of the individuals for whom insurance information is recorded is probably contained in this column. Age plays a significant role in risk assessment and insurance premiums.
    - **Sex:** This column probably indicates the gender of the people, whether they are men or women. The cost of insurance can occasionally be influenced by gender.
    - **BMI (Body Mass Index):** The values for each person's Body Mass Index are listed in this column. Insurance companies frequently use BMI, a number derived from a person's height and weight, to evaluate health risk.
    - **Children:** This column probably lists how many children or other dependents each person has. When it comes to family insurance plans, the number of dependents may be important.
    - **Smoker:** Whether the people are smokers or not is shown in this column. Smoking influences insurance rates because it increases the risk of many different health conditions.
    - **Region:** This column probably contains information about the individuals' locations or regions. Due to variables like healthcare costs and regional regulations, insurance costs can differ by region.
    - **Expenses:** The insurance costs or premiums that each person has likely paid are listed in this column. This is the sum that people pay each year for their insurance coverage.
    
- **Main target columns are Age, Expenses, Smoker but will use all in model development.**
