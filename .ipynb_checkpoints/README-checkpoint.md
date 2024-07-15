# EDA_Bank_Telemarketing_Campaign
 
## Problem statement

The bank provides financial services/products such as savings accounts, current accounts, debit cards, etc. to its customers. In order to increase its overall revenue, the bank conducts various marketing campaigns for its financial products such as credit cards, term deposits, loans, etc. These campaigns are intended for the bank’s existing customers. However, the marketing campaigns need to be cost-efficient so that the bank not only increases their overall revenues but also the total profit. 

A bank conducted a telemarketing campaign for one of its financial products called ‘Term Deposits’ to help foster long-term relationships with existing customers. The dataset contains information about all the customers who were contacted during a particular year to open term deposit accounts with the bank.

What is a term deposit?

Term deposits, also called fixed deposits, are the cash investments made for a specific time period ranging from 1 month to 5 years for predetermined fixed interest rates. The fixed interest rates offered for term deposits are higher than the regular interest rates for savings accounts. The customers receive the total amount (investment plus the interest) at the end of the maturity period. Also, the money can only be withdrawn at the end of the maturity period. Withdrawing money before that will result in penalty charges, and the customer will not receive any interest returns.

## Solution 

		
### Fixing the data types 		
		
		
		
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


	
### Fixing the Rows and Columns 	
	
#### Checklist for Fixing Rows	Description
        Delete summary rows	:Total and Subtotal rows
        Delete incorrect rows:	Header row and footer row
        Delete extra rows:Column number, indicators, Blank rows, Page No.
	
#### Checklist for fixing columns:

        Merge columns for creating unique identifiers, if needed, for example, merge the columns State and City into the column Full address.
        Split columns to get more data: Split the Address column to get State and City columns to analyse each separately.
        Add column names: Add column names if missing.
        Rename columns consistently: Abbreviations, encoded columns.
        Delete columns: Delete unnecessary columns.
        Align misaligned columns: The data set may have shifted columns, which you need to align correctly.


### Impute/Remove missing values 