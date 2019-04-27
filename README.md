# hyperparameter-db-project-db14
hyperparameter-db-project-db14 created by GitHub Classroom

## Abstract
Gather a list of data sets, type of datasets, and hyperparameters by running an expanded list of datasets. This information will be embedded in a database management system, to be incorporated into a website where it is easy to be searched and used by the public.
The hyperparameter database is created by running millions of hyperparameter values, over thousands of public datasets and calculating the individual conditional expectation of every hyperparameter on the quality of a model.
Generate models using H2O software to find the best hyperparameters and create a conceptual model and store all the data into a physical database.

## Objective:
To create Hyperparameter Database by running several hyperparameter values on several datasets and to calculate the individual conditional expectations on every hyperparameter on quality of model

## Data source
Data is derived from Kaggle Datasets. We have chosen considered dataset of Travel Insurance. 

A third-party TRAVEL INSURANCE servicing company that is based in Singapore.
The attributes:
•	Target: Claim Status
•	Name of agency 
•	Type of travel insurance agencies 
•	Distribution channel of travel insurance agencies 
•	Name of the travel insurance products 
•	Duration of travel 
•	Destination of travel 
•	Amount of sales of travel insurance policies 
•	Commission received for travel insurance agency 
•	Gender of insured 
•	Age of insured 

## Conceptual Schema
A conceptual data model identifies the highest-level relationships between the different entities.

## ER Diagram
An entity relationship diagram shows the relationships of entity sets stored in a database. An entity is an object, a component of data. An entity set is a collection of similar entities. These entities have attributes that define its properties.

## Normalization
According to 1NF,  
1. There are no repeating groups  
2. Maintained atomic data values of hyperparameter table is further split into hyperparameter_default and hyperparameter_actual columns 
3. Each field of the table has unique name
4. Each table has primary key 

According to 2NF, 
1. All tables satisfy 1NF 
2. All non-key attributes are dependent on all parts of primary key. Thus, no partial dependencies 3. There are no calculated data
4. Each field of the table has unique name 
5. Each table has primary key 

According to 3NF, 
1. All tables satisfy 2NF 
2. All non-key attributes are not dependent on other non-key attributes. Thus, no transitive relationship 
3. Each field of the table has unique name 
4. Each table has primary key

## Conclusion
Hyperparameter database is built by running several hyperparameter values on Travel Insurance dataset. Data fetched from the dataset is structured into different tables analyzing the relationships between the values. 
Using H20 software, for five run times (500, 1000, 1500, 2000, 2500), respective models and its metrics values are generated. Metrics indicate the absolute fit of the model to actual data. Smaller the metrics values, closer we are to finding the line of best fit. Thus, models generated their own set of hyperparameters. Hence, model architecture is defined for storing the hyperparameter values in the database.






