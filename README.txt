UNCORN COMPANIES
An Exploratory Data Analysis Performed by Nnamdi Leonard

-------------------------------------------------------------------------------------------------------------------
Order Of Execution:
- Business Requirement / Understanding 
- Understanding the Dataset given, and deducing a data dictionary
- Data Cleaning Processes / Transformation
- Analysis and Findings
- Recommendation

-------------------------------------------------------------------------------------------------------------------
BUSINESS REQUIREMENT:

Perform a basic exploratory data analysis of the features of the Unicorn Companies dataset and come up with data 
driven recommendations to help Unicorn Companies in creating good business models and making decisions that will 
focus on companies with high growth potential, diversify investment portfolio and prioritize companies with experienced 
leadership teams.

-------------------------------------------------------------------------------------------------------------------
DATA CLEANING PROCESSES 

* Scanned through the documents by running some queries, below are the steps according to the cleaning process:

- Identified 16 NaN/Null values within the column 'City'. Using the Methods ".loc", and ".replace", I found - 
and replace the null values with the right values after findings were made. I also used same process to replace - 
a null value in the 'Select Investors' column with the right entry after findings were made - same for 'Funding' -
and the 'Year Founded' columns.

- Checked for duplicates; negative.

- Checked for inconsistencies in datatypes, and found that 'Year Founded' was not in a datetime format and corrected it.

- Also had to back-date a particular entry whose date was wrongly entered, using the same replacement method. 


Challenges:
1. Some of these processes was detected as errors in the middle of analysis as they weren't conspicuous. This took-
quite some time and further study to understand the errors and give the desired results.

-------------------------------------------------------------------------------------------------------------------
ANALYSIS 

* A total of eight insights was carried out in this analysis:

1. Unicorn Companies with the biggest return on investment: I had to define a function to extract the numerical - 
values from the 'Funding' and 'Valuation' columns, because the entries were in a complex format. e.g '$nM'.
Afterwards I perfomed a calculation for ROI = [('Valuation' - 'Funding')/'Valuation']*100

2. Time Taken to Become a Unicorn Company: Had to convert the date columns, 'Year Founded' and 'Date Joined' to -
datetime format in order to perform operations of subtraction to arrive at desired result.

3. Fastest Companies to Achieve Unicorn Status: a continuation of the previous step, by setting attribute -
'ascending' to false, I was able to derive some insight.

4. Tech Hub Countries and Cities: Was able to drill down to the number of Unicorn companies in countries and -
cities by the use of 'value_counts()'

5. Investors who Funded The Most Unicorn: Used the same query as above

6. The Companies the Investors Invested In: as a continuation from above, I performed Bivariate analysis to reach -
my results. 

7. Investors Whos spent the Most: used a bivariate analysis for to achieve this.

8. Companies that Received Investments the Most: used a multivariate analysis to achieve this.

-------------------------------------------------------------------------------------------------------------------
RECOMMENDATION:

- A came to a conclusion by giving some recommmendations to the stakeholders based on the insights I derived; which -
are based on improving operations, reducing cost, analysing investments and was to optimize investments to achieve -
increased income.

THANKS FOR YOUR TIME
