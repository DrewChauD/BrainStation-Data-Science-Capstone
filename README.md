### Andrew Chau 
### BrainStation Data Science Capstone Project
### Summer 2023
### Repairability of Consumer Electronics

## Dataset: Open Repair Alliance - https://openrepair.org/open-data/downloads/

# The dataset as of 2023 August contains roughly 100,000 rows and 15 columns
# Data Dictionary:

id: username of the person attempting the repair
data_provider: associated organization overseeing the repairs
country: country in which the repair attempt took place
partner_product_category: includes the general category the product is in
product_category: type of item, categorical
product_category_id: product_category, associated number
brand: manufacturer / brand of the item
year_of_manufacture: year the item was made
product_age: age of the product at the time of the repair attempt
repair_status: item can be listed as "Fixed, Repairable, End of Life, or Unknown"
repair_barrier_if_end_of_life: a description on why the item cannot be repaired
group_identifier: the organization hosting the repair event
event_date: date of the repair event
problem: a description of the issue(s) with the item

## Stakeholders:

Primary manufacturers / businesses: would want to maximize profits and reduce costs arising from loss of reputation
reputation, warranty repairs, switching suppliers, redesign, etc.
Individuals: would want to repair broken electronics for financial, sentimental, and ethical(environmental care) reasons. Less reliance on any supply chain issues is also a plus
Third Party manufacturers / businesses: would want to expand their market for tools, materials, training, merchandise, etc. for the repair industry
Government agencies: would want to meet pollution, waste, climate goals
Global population: generally interested in the conservation of the environment and reduction of its worsening

## Problem Space: When consumer e lectronics are discarded, they generate not only toxic landfill waste but also pollution at the resource extraction, manufacturing, transportation, packaging, and point-of-sale stages.


## Proposed solutions: 

# Repairing consumer electronics can be quick, cost-effective, and rewarding, but the unknown aspects can make this task seem like a gamble. Analysis of the dataset using regression / classification of the numerical values, and/or NLP for the text column would remove uncertainty and provide guidance on how feasible a repair might be. Empowering people with this information can lead to a higher willingness to engage in repair. 