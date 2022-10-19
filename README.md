# Cleaning Data in SQL

## Overview  
This project is aimed at cleaning Nashville Housing Data using SQL. I first explored the data and checked for data quality, then fixed errors, 
filled in some missing values where applicable, changed data types where necessary, created new columns and splitted some columns, 
removed duplicate data and deleted unwanted columns.  
The Data used contained (56,477 rows) before cleaning. It is provided in the repository. 

## Database and Tool used:  
* Microsoft SQL Server 
* SQL Server Management Studio

## Skills and Steps deployed:  
* Standardized Date Format:  
The "SaleDate" Column is in DATETIME format, and I am only interested in the DATE part of it. So i used CONVERT() function for this operation.

* Broke-out Address into Individual Columns:  
 Using SUBSTRING, CHARINDEX, PARSENAME and REPLACE functions, I splitted the "PropertyAddress" column into (Address, City, State)  
 
 * Changed Y and N to Yes and No in "Sold as Vacant" field:  
 I used CASE STATEMENT to replace  Y with Yes and N with No in the "Sold as Vacant) column.
 
 * Removed Duplicate Data:  
 Got rid of duplicate data using ROW_NUMBER, CTE, ORDER BY,  And windows function of PARTITION BY. After which the data came down to 56,373
 
 * Deleted Unwanted Columns:  
 Finally, I deleted columns that are irrelevant and unwanted.
 
 ## CONTACT:
 For project, collaboration, recommendation, or correction on my work, please reach out to me on the following:
* hafizdabo@gmail.com 
* +2348039138334 | call and whatsapp
* https://wwww.linkedin.com/in/hafizdabo
