# HR ANALYTICS DASHBOARD

## Problem Statement

This dashboard helps to understand the Data For HR which gives the employment information of the employees. It includes Attrition,Business Travel, age group,department,education,employee number ,gender,job role ,martial status,over time,age over 18 or not,training time last year,age,distance currently from home,currently employeed or notincome,working hours and other columns.  
###Steps Followed

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Check the columns and header of the columns were not given ,so first row as headers were used.
- Step 4 : After transforming the data , clicked on close and apply from home tab.
- Step 5 :In the report view, under the view tab, theme was selected.
- Step 6 : New Column named Attrition Count was added. The condition taken was that if the Attrition is Yes,the output will be 1,else 0.
- Step 7 : A measure was added using DAX named as Attrition Rate.
- Step 8 :  Again a new measure was created named as Active Employees.
- Step 9 : KPI's  were added for :"Total Employees","Attrition","Attrition Rate","Active Employees", "Average Age".
- Step 10 : A pie chart was created in which Sum of Attrition Count was taken in values and in Legend Department was taken.
- Step 11 : A Column Chart was created representing No of Employees by Age Group with respect to gender. So gender was taken in Legend Field.
- Step 12 : Sorting for the above graph according to age had to done. So we will add a column named as "Sort Age" with conditions if age band is  under 25,output will be 1 and if age band is 25-34 ,output will be 2 and so on. Then on the graph and sorting was done according to sort age in ascending order.
- Step 13 : A Matrix was created giving relationship between  Job Role and Job Satisfaction and sum of employees count will be taken in values.
- Step 14 - A bar chart was created for sum of attrition count  by education field.
- Step 15 - Donut Chart were created for Attrition Rate of gender by each age group.
- Step 16 - For each donut chart in above step gender was taken on legend ,sum of attrition count was taken on values and cf_age band was taken in details and filtering will be done according to age.
- Step 17 - Then in each donut chart, card was added indicating the attrition of particular age group.
- Step 18 - Slicers were added for Education which will segregate the graphs according to Education.

###DAX Expressions used for creating Measures for Card Visuals.
- 1)Attrition Rate = SUM('HR data'[Attrition count])/SUM('HR data'[Employee Count])
Snap of Attrition Rate: 
![attrition rate](https://github.com/Shreyavig/HR-DATA-ANALYTICS/assets/158707069/59a40a7d-e94c-4487-a7ac-18bc6a571d0b)

- 2)Active Employees = SUM('HR data'[Employee Count])-SUM('HR data'[Attrition count])
Call-Centre-Dashboard/assets/158707069/8517111e-c3ae-46f1-aca5-c67cd06aadd5)
Snap of Active Employees :
![Active employees](https://github.com/Shreyavig/HR-DATA-ANALYTICS/assets/158707069/53343b52-a664-4896-b6c7-0de0c7ed455c)

### Snaps of cards,slicers used in Dashboard
1)Total Employees:
![total employees](https://github.com/Shreyavig/HR-DATA-ANALYTICS/assets/158707069/5e410f5a-9105-44e5-8e85-38938135bf23)

2)Attrition:
![Attrition](https://github.com/Shreyavig/HR-DATA-ANALYTICS/assets/158707069/ec65347b-2bbd-4529-b8b9-dfc89b2bef60)

3) Average Age :
![average age](https://github.com/Shreyavig/HR-DATA-ANALYTICS/assets/158707069/0407bfc2-2853-4449-bc03-1bf190114b2d)

### Slicers 

![Slicers](https://github.com/Shreyavig/HR-DATA-ANALYTICS/assets/158707069/d3d7b433-b3c0-4b6d-acdd-03253de6521b)
407bfc2-2853-4449-bc03-1bf190114b2d)

### Snap of Power Bi Dashboard

![hr ss](https://github.com/Shreyavig/HR-DATA-ANALYTICS/assets/158707069/57a3a7e6-ed65-485e-ae4c-4a3a92c223f9)









