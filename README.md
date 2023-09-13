## Andrew Chau 
### kuzals@gmail.com
### https://github.com/DrewChauD/
### BrainStation Data Science Capstone Project
### Summer 2023
### Repairability of Consumer Electronics

## Dataset: Open Repair Alliance - https://openrepair.org/open-data/downloads/ - OpenRepairData_v0.3_aggregate_202303.csv

### The dataset as of August 2023 contains roughly 100,000 rows and 15 columns

# Data Dictionary:

id: username of the person attempting the repair <br>
data_provider: associated organization overseeing the repairs <br>
country: country in which the repair attempt took place <br>
partner_product_category: includes the general category the product is in <br>
product_category: type of item, categorical <br>
product_category_id: product_category, associated number <br>
brand: manufacturer / brand of the item <br>
year_of_manufacture: year the item was made <br>
product_age: age of the product at the time of the repair attempt <br>
repair_status: item can be listed as "Fixed, Repairable, End of Life, or Unknown" <br>
repair_barrier_if_end_of_life: a description on why the item cannot be repaired <br>
group_identifier: the organization hosting the repair event <br>
event_date: date of the repair event <br>
problem: a description of the issue(s) with the item <br>

## Problem Space: 

When consumer electronics are discarded, they generate not only toxic landfill waste but also pollution at the resource extraction, manufacturing, transportation, packaging, and point-of-sale stages. <br>
Additionally, stagnant wages and rising costs of living put increasing financial pressures on families and individuals when they choose to replace malfunctioning consumer electronics. <br>
Furthermore, the global supply chain is still recovering from the effects of the COVID-19 pandemic and currently very susceptible to disruption, leading to shortages and delays in bringing consumer electronics from raw materials to manufacturing to transportation to a finished product ready for purchase

## Stakeholders:

Raw material extractors: Reduces burden on resources extractors who lately have had to turn to increasingly expensive, dangerous, and inefficient methods <br>
Primary manufacturers / businesses: would want to maximize profits and reduce costs arising from loss of reputation, warranty repairs, switching suppliers, redesign, etc.<br>
Individuals: would want to repair broken electronics for financial, sentimental, and ethical(environmental care) reasons. Less reliance on any supply chain issues is also a plus<br>
Third Party manufacturers / businesses: would want to expand their market for tools, materials, training, merchandise, etc. for the repair industry<br>
Government agencies: would want to meet pollution, waste, climate goals<br>
Global population: generally interested in the conservation of the environment and reduction of its deterioration<br>


## Impact of Proposed Solutions: 

Repairing consumer electronics can be quick, cost-effective, environmentally friendly, and rewarding, but the unknown aspects can make this task seem like a gamble. <br>
Analyzing the dataset using decision-tree methods on key columns as well as NLP for the text column can provide answers that will remove uncertainty and provide guidance on how feasible a repair might be. <br>
Empowering people with this information can lead to a higher willingness to engage in repair. Repairing rather than discarding consumer electronics would reduce waste and pollution, create value, and greatly expedite the acquisition of a functioning item

## Notebooks: 

Notebook #1 - Andrew_Chau_BrainStation_DS_Capstone_Book_1_EDA.ipynb

* Introduction
* Dataset Information
* Exploratory Data Analysis Part 1 of 2
 - shape, datatypes, distribution, close-up look at the data
 - data cleaning
* Exploratory Data Analysis Part 2 of 2
 - looking at count of values
 - relationship between columns
 - visual representation of findings

Notebook #2 - Andrew_Chau_BrainStation_DS_Capstone_Book_2_Modeling.ipynb

* Data preprocessing for Decision-Tree Modeling
 - feature selection
 - reduce Target Variable column down from 4 values to 2
 - data transformation (one-hot encoding, dummy variables, sparse matrix)
 - balancing classes (downsampling)
* Decision-Tree Modeling
 - Sci-kit Learn DecisionTreeClassifier
 - Presenting the results in confusion matrices in both numeric and visual forms
* Data preprocessing for Natural Language Processing
 - Further data cleaning to only include English
 - reduce Target Variable column down from 4 values to 2
 - Sci-kit Learn CountVectorizer
 - Determining how much of the data to include in the model
 - Removing English stop words
 - Lemmatization of remaining words
* Natural Language Processing Modeling (Logistic Regression)
 - Logistic Regression
 - Determining and displaying the coefficients for positive and negative words
 - Presenting the results in confusion matrices in both numeric and visual forms
 - Attempt at XGBoost for increased performance
 - Hyperparameter tuning, grid search, bagging, boosting

* Leading Model Evaluation
 - Performance evaluation versus baseline
 - Reflections on model optimization process

* Conclusion
 - Model suitability to solve the listed problem
 - Impact of using the model
 - Next steps