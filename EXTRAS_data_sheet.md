# Datasheet Template


## Motivation

- For what purpose was the dataset created? 
The dataset was developed to support comercial campaigns  related to sreaming products in order to identify the most valuables customers who will probably after a free period of streaming will continue sot subscribe Disney+

- Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?

The dataset was developed by our analytics team in collaboration with Data Science Team and Product Managment inputs for comercial purposes like for example to identify after which period a customer is profitable in that specific product.

 
## Composition

- What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)? 
- How many instances of each type are there? 
- Is there any missing data?
- Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?

The dataset contains information about customers from the past two years. Although all data has been modified for this project and customers have been anonymized, this dataset is not public. Therefore, please do not forward it under any circumstances.


## Collection process

- How was the data acquired? 
- If the data is a sample of a larger subset, what was the sampling strategy? 
- Over what time frame was the data collected?

We take three snapshots to train the data and an additional snapshot for final evaluation of the model as described below. Data is a sample of 3 months considering the most recent data available and also the necessary window to measure the target .
 




## Preprocessing/cleaning/labelling

- Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section. 
- Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)? 


The preprocessing process for the dataset involved several critical steps to ensure the data was suitable for modeling. First, null values were addressed appropriately to maintain data integrity. This involved imputing missing values using methods such as calculating and inserting median values where applicable.

Next, categorical variables were summarized to condense and represent the information effectively. This step often included encoding categorical variables into numerical formats suitable for analysis.

Additionally, date features were removed from the dataset to avoid potential biases or overfitting that could arise from time-related data.

Finally, the dataset was balanced to ensure equal representation of data across the months utilized. This balancing act was crucial to prevent any temporal skew and to ensure the model received a uniform distribution of data over the specified period.
 
## Uses

- What other tasks could the dataset be used for? 
- Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms? 
- Are there tasks for which the dataset should not be used? If so, please provide a description.

Currently, our dataset reflects only one type of subscription. Should different categories of subscriptions, such as Prime or Standard, be introduced in the future, the dataset will require a thorough review and update. The introduction of varied subscription types is likely to influence customer behavior significantly, affecting their decision to continue paying for the service. Consequently, it will be essential to reevaluate and preprocess the dataset to account for these new subscription categories, ensuring that the model accurately reflects and adapts to these changes in customer behavior.

## Distribution

- How has the dataset already been distributed? 
- Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?  

It is not public as it contain customer information .

## Maintenance

- Who maintains the dataset?

The dataset is maintained in an automated manner, with new information being fed into the system daily. As a result, the model undergoes continuous re-evaluation to incorporate the latest data. This automated process ensures that the dataset remains up-to-date and that the model's performance is consistently optimized in response to the most recent information available.
