# EDA_Bank_Telemarketing_Campaign
 
## Problem statement

The bank provides financial services/products such as savings accounts, current accounts, debit cards, etc. to its customers. In order to increase its overall revenue, the bank conducts various marketing campaigns for its financial products such as credit cards, term deposits, loans, etc. These campaigns are intended for the bank’s existing customers. However, the marketing campaigns need to be cost-efficient so that the bank not only increases their overall revenues but also the total profit. 

A bank conducted a telemarketing campaign for one of its financial products called ‘Term Deposits’ to help foster long-term relationships with existing customers. The dataset contains information about all the customers who were contacted during a particular year to open term deposit accounts with the bank.

What is a term deposit?

Term deposits, also called fixed deposits, are the cash investments made for a specific time period ranging from 1 month to 5 years for predetermined fixed interest rates. The fixed interest rates offered for term deposits are higher than the regular interest rates for savings accounts. The customers receive the total amount (investment plus the interest) at the end of the maturity period. Also, the money can only be withdrawn at the end of the maturity period. Withdrawing money before that will result in penalty charges, and the customer will not receive any interest returns.

## Solution 

### Data Cleaning
		
#### Fixing the data types 		
		
		
		
    Data Type	                         Description	                             Examples
    Numeric	                             Quantitative data	                       Age, income, temperature
    Categorical (Nominal)	             Categories without inherent order	       Gender, country
    Categorical (Ordinal)	             Categories with inherent order	           Rating, education level
    Time and Date	                     Dates and times	                       Date of birth, appointment time
    Coordinates	                         Geographical data	                       Latitude, longitude
    Boolean	                             Binary data	                           True/False, Yes/No
    Text	                             Strings of text	                       Names, addresses
    Complex	                             Complex numbers	                       3 + 4i, 5 - 2i
    Image	                             Image data	                               JPEG, PNG
    Binary	                             Binary data	                           Files, multimedia data
    Object	                             Mixed data types	                       Lists, dictionaries


	
#### Fixing the Rows and Columns 	
	
##### Checklist for Fixing Rows	Description
        Delete summary rows	:Total and Subtotal rows
        Delete incorrect rows:	Header row and footer row
        Delete extra rows:Column number, indicators, Blank rows, Page No.
	
##### Checklist for fixing columns:

        Merge columns for creating unique identifiers, if needed, for example, merge the columns State and City into the column Full address.
        Split columns to get more data: Split the Address column to get State and City columns to analyse each separately.
        Add column names: Add column names if missing.
        Rename columns consistently: Abbreviations, encoded columns.
        Delete columns: Delete unnecessary columns.
        Align misaligned columns: The data set may have shifted columns, which you need to align correctly.


#### Impute/Remove missing values 

    Set values as missing values: Identify values that indicate missing data, for example, treat blank strings, "NA", "XX", "999", etc., as missing.
    Adding is good, exaggerating is bad: You should try to get information from reliable external sources as much as possible, but if you can’t, then it is better to retain missing values rather than          exaggerating the existing rows/columns.
    Delete rows and columns: Rows can be deleted if the number of missing values is insignificant, as this would not impact the overall analysis results. Columns can be removed if the missing values are       quite significant in number.
    Fill partial missing values using business judgment: Such values include missing time zone, century, etc. These values can be identified easily.
    Types of missing values:
    
    MCAR: It stands for Missing completely at random (the reason behind the missing value is not dependent on any other feature).
    MAR: It stands for Missing at random (the reason behind the missing value may be associated with some other features).
    MNAR: It stands for Missing not at random (there is a specific reason behind the missing value).


#### Handling Outliers 

Major approaches to the treat outliers:
 		
     Imputation
     Deletion of outliers
     Binning of values
     Cap the outlier
    
#### Standardising values 

    Standardise units: Ensure all observations under one variable are expressed in a common and consistent unit, e.g., convert lbs to kg, miles/hr to km/hr, etc.
    Scale values if required: Make sure all the observations under one variable have a common scale.
    Standardise precision for better presentation of data, e.g., change 4.5312341 kg to 4.53 kg.
    Remove extra characters such as common prefixes/suffixes, leading/trailing/multiple spaces, etc. These are irrelevant to analysis.
    Standardise case: String variables may take various casing styles, e.g., UPPERCASE, lowercase, Title Case, Sentence case, etc.
    Standardise format: It is important to standardise the format of other elements such as date, name, etce.g., change 23/10/16 to 2016/10/23, “Modi, Narendra” to “Narendra Modi", etc.



### Univariate Analysis 

#### Categorical unordered univariate analysis 

    Unordered data do not have the notion of high-low, more-less etc.
    Example:
    
    Type of loan taken by a person = home, personal, auto etc.
    Organisation of a person = Sales, marketing, HR etc.
    Job category of persone.
    Marital status of any one.


#### Categorical ordered univariate analysis 

    Ordered variables have some kind of ordering. Some examples of bank marketing dataset are:

    Age group= <30, 30-40, 40-50 and so on.
    Month = Jan-Feb-Mar etc.
    Education = primary, secondary and so on.



### Bivariate and Multivariate Analysis

    Numeric- numeric analysis
        There are three ways to analyse the numeric- numeric data types simultaneously.
        
        Scatter plot: describes the pattern that how one variable is varying with other variable.
        Correlation matrix: to describe the linearity of two numeric variables.
        Pair plot: group of scatter plots of all numeric variables in the data frame.


    Numerical categorical variable

    Categorical categorical variable 

### Multivariate analysis 