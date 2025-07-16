Excel#4

Project Description

Excel-4 shows practical examples of data validation in Excel. Here you'll find tips, instructions, and illustrations about validating data and creating drop down tables.

Table of Contents 

Data validation

In this example we will be checking whether entered value is between 1 and 10.
To create the data validation rule, execute the following steps:
1. Select cell B1.
2. On the Data tab, in the Data Tools group, click Data Validation.
On the Settings tab:
3. In the Allow list, click Whole number, In the Data list click between.
4. Enter Maximum and Minimum values.
![screenshot](Screenshots/Validation.png)
Input Message window:
![screenshot](Screenshots/Input.png)
Error Alert window:
![screenshot](Screenshots/Error.png)

Results:
When user selects cell B1:
![screenshot](Screenshots/Result.png)
When user enters number from range 1-10 everything is fine:
![screenshot](Screenshots/Result1.png)
When user enters number out of range:
![screenshot](Screenshots/Result2.png)

(Note: to remove data validation from a cell, select the cell, on the Data tab, in the Data Tools group, click Data Validation, and then click Clear All)

Budget limit example

To avoid exceeding a budget limit in Excel use data validation and the SUM function.

1. Select range E2:E6 and click Data Validation.
2. In the Allow list, click Custom.
3. In the formula box enter: =SUM($E$2:$E$6)<=80
![screenshot](Screenshots/Validation1.png)
Result when user exceeds budget:
![screenshot](Screenshots/Result3.png)

Prevent duplicates example

1. Select range G2:G15 and click Data Validation
2. In the Allow list, click Custom.
3. In the formula box enter: =COUNTIF($G$2:$G$15;G2)=1
![screenshot](Screenshots/Validation2.png)
(Note: we count the number of values in range G2:G15 that are equal to value in cell G2. This value may occur only once. Because we selected range G2:G15 before we selected Data Validation, Excel automatically copies the formula to the other cells. Absolute reference $G$2:$G$15 stays locked.)
Result:
![screenshot](Screenshots/Result4.png)

Drop-down lists

1. On the first sheet type food names:
![screenshot](Screenshots/List.png)
2. On the second sheet select cell B1 then click Data Validation.
3. In the Allow box, click List.
4. Click in the Source box and select the range I1:I4 on the first sheet.
![screenshot](Screenshots/List1.png)
5. Click OK
![screenshot](Screenshots/List2.png)
