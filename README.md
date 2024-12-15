# Data-Wrangling

# Data Wrangling Report for Customer Analytics at XYZ Company

# Project Objective:

The main objective of this project was to do extensive data wrangling in order to create a solid dataset for customer analytics at XYZ company. This involved cleaning, transforming, and integrating consumer data from various sources to improve its accuracy, usability, and efficacy for future analysis and reporting.

# Background and Need for Data Wrangling.
XYZ Company has collected a huge quantity of client data through multiple channels, such as sales transactions, customer support encounters, and marketing initiatives. However, this data is filled with discrepancies, missing values, and fragmentation, making it difficult to draw significant conclusions. Effective data management was required to develop a consolidated and clean dataset, allowing for more targeted and successful marketing strategies and better decision-making.

# Data Sources:

The data wrangling procedure required working with several datasets, including:

- Sales Data: Transaction records include client IDs, purchase amounts, product descriptions, and timestamps.

- Customer demographics include age, gender, geography, and account creation date.

- Client Service Records are logs of client enquiries, complaints, and resolutions.

- Marketing Interaction Data: Email and campaign response statistics, such as open and click-through rates. 

# Methodology

The data wrangling process followed these key steps:

- Data Collection. I collected the essential data from online. All relevant datasets were collected and aggregated to provide a comprehensive client profile.

- Data Assessment. An initial data quality evaluation was carried out to detect issues including missing values, duplication, and conflicts between datasets. This assisted in determining the level of cleaning and transformation required.

- Data Cleaning

● Missing Values: I handled missing values by using approaches such as imputation for numerical fields and exclusion when data could not be properly imputed.

● Duplicates and Inconsistencies: I removed duplicate records and standardised inconsistent data formats, such as date formats and naming standards (for example, gender and status values).

● Categorical Data Normalisation: To guarantee uniformity among datasets, categorical variables (such as "active" and "inactive") were normalised.

- Data Transformation

● Data Type Conversion: I transformed fields into suitable formats for analysis, such as converting strings into date and time objects for easier processing.

● New Feature Derivation: Features such as total purchase amounts, frequency of purchases, and customer tenure were developed to improve analytical capabilities.

● Data Aggregation: Data was aggregated to meet analysis requirements, such as summarising monthly sales by customer.

- Data Consolidation. I combined datasets into a single customer database, connecting them with unique identifiers such as customer ID. This aggregation enabled me to build a full image of each customer by merging sales, service, and marketing data.

# Documentation and Validation

I documented the entire data-wrangling process, including the sources, cleaning methods, and transformations used. The final dataset was evaluated using exploratory data analysis (EDA) to guarantee accuracy and completeness.

# Tools and Technologies Used

The following tools and technologies were employed throughout the data wrangling process.

Python (Pandas, NumPy): For data manipulation and cleanup.

Matplotlib with Seaborn: Used for data visualisation, EDA, and quality assurance.

# Deliverables

The following deliverables were created:

- Cleaned and Transformed Dataset: A dataset prepared for analysis in CSV format. This dataset is now consistent, accurate, and well-organised for consumer analytics.

- Comprehensive Report: A detailed report that describes the data wrangling process, methodologies used, obstacles faced, and major properties of the final dataset.- 

- Visualisations include charts and graphs that depict data insights such as missing value distributions, outliers, and key correlations between variables. This helps to check the data's quality and completeness.


Data Summary:
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 10 entries, 0 to 9
Data columns (total 5 columns):
 #   Column                 Non-Null Count  Dtype  
---  ------                 --------------  -----  
 0   customer_id            10 non-null     int64  
 1   customer_age           9 non-null      float64
 2   total_purchase_amount  9 non-null      float64
 3   customer_status        10 non-null     object 
 4   account_creation_date  10 non-null     object 
dtypes: float64(2), int64(1), object(2)
memory usage: 528.0+ bytes
None

Missing Values:
customer_id              0
customer_age             1
total_purchase_amount    1
customer_status          0
account_creation_date    0
dtype: int64

Cleaned Data Summary:
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 10 entries, 0 to 9
Data columns (total 5 columns):
 #   Column                 Non-Null Count  Dtype  
---  ------                 --------------  -----  
 0   customer_id            10 non-null     int64  
 1   customer_age           10 non-null     float64
 2   total_purchase_amount  10 non-null     float64
 3   customer_status        10 non-null     object 
 4   account_creation_date  10 non-null     object 

 	customer_id	customer_age	total_purchase_amount	customer_status	account_creation_date	customer_tenure
0	1	25.0	1200.5	active	2021-01-01	3
1	2	32.0	1500.0	inactive	2020-06-15	4
2	3	47.0	2000.3	active	2019-07-20	5
3	4	54.0	800.5	inactive	2018-05-10	6
4	5	23.0	500.2	active	2021-02-05	3


Consolidated Data:
   customer_id  customer_age  total_purchase_amount customer_status  \
0            1          25.0                 1200.5          active   
1            2          32.0                 1500.0        inactive   
2            3          47.0                 2000.3          active   
3            4          54.0                  800.5        inactive   
4            5          23.0                  500.2          active   

  account_creation_date  customer_tenure  
0            2021-01-01                3  
1            2020-06-15                4  
2            2019-07-20                5  
3            2018-05-10                6  
4            2021-02-05                3  

![image](https://github.com/user-attachments/assets/d33265a9-9e94-4266-a9f6-8f1dcabce6c9)

![image](https://github.com/user-attachments/assets/e38b0019-f66d-4a8a-87b0-72a9da9b437b)

![image](https://github.com/user-attachments/assets/3ea71c4a-8737-41ef-aae3-280c592854fa)

![image](https://github.com/user-attachments/assets/2b1b6e2c-26c6-47f9-ac87-26984bcff52a)

![image](https://github.com/user-attachments/assets/352f7c9f-387f-4ff5-b670-132c22aa5b12)

![image](https://github.com/user-attachments/assets/a0a006f0-3ff7-49fa-9fd7-7ae3d48b2482)

# Challenges Encountered

During the data wrangling process, faced several challenges:

Inconsistent Data forms: Some datasets used different forms for date fields and categorical variables, necessitating extensive normalisation.

Missing Data: Several records were lacking demographic or transactional information, necessitating cautious imputation or exclusion.

Duplicate Records: Some datasets included duplicate items that needed to be detected and eliminated.

# Conclusion

The data wrangling process provided a clean, comprehensive, and well-organised customer dataset that will serve as the foundation for XYZ Company's customer analytics efforts. By correcting data discrepancies, cleansing missing or incorrect information, and consolidating the data into a consistent format, I improved its correctness and usability for further analysis.
Moreover, this cleaned dataset will allow XYZ Company to conduct more effective consumer segmentation, targeted marketing, and data-driven decision-making. The report, combined with the visualisations and documented process, presents a clear and thorough picture of the data wrangling activities carried out to assure high-quality data for future analytics.










