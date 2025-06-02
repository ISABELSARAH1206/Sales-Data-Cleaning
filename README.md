# SALES DATA CLEANING  
This exercise is carried out to solidify my data cleaning skill.  
The dataset used here, is taken from kaggle.  
The raw dataset is a CSV file made up of 15 columns and 7395 rows, including header and blank rows Below are the columns of the dataset and their data types.  
## PREVIEW OF THE RAW DATA
![image](https://github.com/user-attachments/assets/9bbd2454-bbe3-43d5-9e15-9ec3cae150f7)  
# DATA CLEANING PROCESSES USING MS EXCEL  
## 1. Autofit  
In the left side corner , there's a triangle between the columns and rows. Click the triangle , to select all the columns and rows . After selecting all the rows and columns , move the mouse between the column labels , until the double-headed arrow appears. When the double-headed arrow appears, double-click to autofit columns . Do the same for rows.  
AFTER:  
![image](https://github.com/user-attachments/assets/d67182da-22d8-4a4a-aad6-8d0266a64027)  
## 2. Remove Duplicates  
To remove duplicates , select all columns and rows or select the desired columns , and go to home -> click conditional formatting -> click highlight cell rules-> click duplicate values -> select the desired colour to highlight duplicate values  
![image](https://github.com/user-attachments/assets/b6df5873-0a1f-4970-8269-83b948a0ae45)  
![image](https://github.com/user-attachments/assets/3fbe7e59-6c43-4b2e-809d-44e88310ecda)  
I have selected the A column to check whether there are any duplicate values . Gladly! there isn't any.  
But if there are any duplicates , it will be highlighted and if u want to remove those duplicates, go to Data tab -> click remove duplicates   
## 3. Blank cells  
to check whether there are any blank cells, select the desired columns and go to home tab-> go to find & select -> click go to special  
![image](https://github.com/user-attachments/assets/20b1014a-e17b-4d27-aa63-14f1961e4218)  
select blank cells -> click ok  
![image](https://github.com/user-attachments/assets/bbe83291-c3d0-4e3e-ab08-0120ba09791b)  
The MS Excel will check and tell if there are any blank cells . As for me , i got zero blank cells.  
![image](https://github.com/user-attachments/assets/837c12ad-07f6-4b36-a3d2-a35fbd9ce829)  
But if you have blank cells, type any value or texts and then click ctrl+enter to enter the same in other blank cells  
## 4. Check spelling  
To check whether there are any spelling errors in the dataset, select the desired columns and go to review tab -> click spelling   
![image](https://github.com/user-attachments/assets/5301540c-541d-4e7a-bd0f-94995161739c)  
I've got no spelling mistakes .  
## 5. Find and Replace  
To replace the desired columns or lines , select the desired columns -> go to home tab -> click find & replace  
![image](https://github.com/user-attachments/assets/6604bc3c-acc6-49ec-b056-da87460052fd)  
type the existing text or value in the "find what" and the text or value that should be replaced in the "replace with "   
## 6. Sort  
we can sort the elements by making a table and then click the arrow near the header , and then click sort A to Z or click old to new or click new to old  

# QUERIES RELATED TO ABOVE WORK  
1. **What are missing values, and how do you handle them?**  
Missing values occur when cells are empty or contain placeholder values like "NA" or "N/A".  
How to handle in Excel:  
Filter and Remove: Use filters to locate blank cells and remove them.  
Fill with Values: Use IF or IFERROR functions to fill missing data.  
Interpolation: Fill blanks using trends or averages in Excel.  

2. **How do you treat duplicate records?**  
Duplicate records can be redundant or errors.  
Steps in Excel:  
Select the data.  
Go to Data > Remove Duplicates.  
Flagging:  
Use conditional formatting to highlight duplicates:  
Home > Conditional Formatting > Highlight Cell Rules > Duplicate Values.  

3. **Difference between dropna() and fillna() in Pandas?**  
In Excel:  
dropna() Equivalent: Delete rows/columns with blanks.  
Filter data by blanks (Filter by Blanks) and delete.  
fillna() Equivalent: Replace blanks with specific values.  
Use Find and Replace (Ctrl + H) to replace blanks with a default value.  

4. **What is outlier treatment, and why is it important?**  
Outliers are extreme values that may distort analysis.  
In Excel:  
Use the =QUARTILE() function to calculate Q1, Q3, and IQR.  
Replace: Use a formula to replace outliers with mean or median values.  
Remove: Manually filter outliers based on calculated thresholds.  

5. **Explain the process of standardizing data.**  
Standardizing scales data for uniformity.  
In Excel:  
Calculate the mean and standard deviation using =AVERAGE(range) and =STDEV.P(range).  
Use the formula:  
Standardized Value=  
(Original Value - Mean)  
Standard Deviation  
Standardized Value=   
Standard Deviation  
(Original Value - Mean)  

6. **How do you handle inconsistent data formats (e.g., date/time)?** 
Steps in Excel:  
Date/Time Formatting:  
Highlight the column, right-click, and select Format Cells.  
Choose a consistent format (e.g., YYYY-MM-DD).  
Text to Columns:  
Use Data > Text to Columns to split and reformat inconsistent data.  
Functions:  
Use TEXT() to convert formats.  
Example: =TEXT(A2,"YYYY-MM-DD").  
Use DATEVALUE() or TIMEVALUE() to convert text dates/times to proper formats.  

7. **What are common data cleaning challenges?**  
In Excel:  
Missing Data: Handled with filters, conditional formulas, or averages.  
Duplicate Records: Found and removed using the Remove Duplicates tool.  
Inconsistent Formats: Standardized with TEXT() and formatting tools.  
Large Datasets: Excel may slow down with large datasets; use pivot tables or summarize data first.  

8. **How can you check data quality?**  
In Excel:  
Use Descriptive Statistics: Use the Data Analysis ToolPak (add-in) to generate descriptive statistics.  
Conditional Formatting:  
Highlight invalid or missing entries.  
Error Checks:   
Use ISERROR() or ISNUMBER() to validate data types.  
Example: =IF(ISNUMBER(A2), "Valid", "Invalid").  
Visualization:  
Create charts like histograms or box plots to spot anomalies.  
Excel provides a user-friendly way to clean, analyze, and visualize data effectively.  
