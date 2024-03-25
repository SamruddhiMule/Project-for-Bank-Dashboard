


# SM Bank-Dashboard

### Dashboard Link :https://app.powerbi.com/groups/me/reports/478ae663-456a-4dab-a0d4-bf6eaa457e1a/ReportSection?experience=power-bi

## Problem Statement

This Dashboard helps the Bank owner understand their customers better. It helps the Bank know if their customers are satisfied with their services. Through different schemes, they get to know top customers, & thus they can improve their services. It also lets them know the average balance in Bank, thus since by using this dashboard they have identified this problem, they can further work on factors responsible for increasing in investmens and giving beneficiary schemes.

Since, number of customers of age above 50 to save money in Bank are less (less than 332 out of 4014)  while avrage age for customers with maximum balance are 35 and 30 ( with count of customer around 790), thus in all they must work on providing better schemes to elderly customers with their services. 


### Steps followed :

- Step 1 : Load data into Power BI Desktop, dataset is a csv file.
- Step 2 :Once dataset is loaded ensure dataset name and columns from right side otion of data.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns errors & empty values were present.
- Step 5 : For calculating total customers in bank score card visual added using the ellipses in the visualizations pane in report view.
- Step 6 : In Build visual from visualizations select "Customer ID" as field and on dropdown option select option as Count."Total Customers" will display in 1st Card visual.
New measure was created to find total count of customers.

Following DAX expression was written for the same,
        
        Count of Customers = COUNT(Bank_data[Customer_ID])
        
A card visual was used to represent count of customers

 ![image](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/694dc5da-b3bb-4e47-8340-a916893cf312)



- Step 7 : Since the data contains various Customers are from differnt areas, Gender and Job Classifications. Thus in order to represent Top customer with highest balance, another visual Score card was added using card option in the visualizations pane in report view. 


- Step 8 : In Build visual from visualizations select "Balanace" as field and on dropdown option select option as SUM."Total Balance" will display in 2nd Card visual

  
Following DAX expression was written to find total Balance,
 
         Total Balance In Bank = SUM(Bank_Data[Balance])
    
 
 
 
 ![TotalBalance](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/8bf9959d-ccc1-434e-9885-3b8227133b4e)




- Step 9 : Another one card visuals were added to the canvas, representing Name of cutomer with maximum balance as "Top Customer". This will help Bank to design scheme for cutomer with highest balance.

  ![image](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/bea13083-d3ab-4964-9faf-446e04091946)


 Using visual dropdown option as "first" from pane, basic filtering was used & null values were unselected for consideration into calculation.
           
   Although, by default, while calculating average, blank values are ignored.

- Step 10 : A Bar chart was also added to the report design area representing the number of customers joined in the Bank as per differnt months. While creating this visual, field named "Customer ID" with count dropdown otion on y-axis and "Date Joined" with only year and moths option on X-axis were also added to the fields, thus number of customers are also seggregated according the gender. 




 
   ![JCusMonths](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/8b90b808-505d-47f1-aa1c-eb4db3a499cd)





- Step 11 : A Pie chart Visual is also added to get percentage vise customers on the basis on Gender.
  


  ![image](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/dfb503bd-4444-41be-b07d-f6af691ff970)




- Step 12 : For better understanding of customers "Region" attribute is used and to representing it with Map Visual.


  ![image](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/242ce891-77ec-404d-a73a-0cfd4d2a7417)




In the SM Bank Dashboard one Page added as Observation.
The insert tab used to insert a text box on 2nd page of SM Bank Dashboard, which has Text as " Highest Customer are from white coller Job classification" which is one of the observation comprehended from dashboard's Visualization.

 ![imageWhite-Collar](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/f5e848db-ab27-4d99-b56f-dbc6359f97ce)



After above process selected View option from tab and made Bookmark by clicking on Add Bookmark.
 

 ![image](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/bff30f53-32dd-4591-bd1b-4c307f0dd76b)

 
 
 Another three text boxes inserted with observations as belows:

2)" lowest Customer are from Other Job classification" 
 


![imageOthers](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/9b822359-8d1c-4ce7-a37f-8a89a2941920)
 

3)" SM Bank Data for Male Customers with 2nd Highest job classification as Blue Collar"
 


![GenderM](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/16b2fc5e-08f6-4236-9ff5-dedee88276b6)



4)" SM Bank Data for Female Customers with 2nd Highest job classification as Other."



  ![GenderF](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/84e6017d-8044-49a0-b613-dc4c4f7f3f93)


After above process, selected View option from tab and made Bookmarks for remaning 3 Observation by clicking on Add Bookmark.

- Step 13 : On that Same  Observation Page four buttons added in frount of each Observation to give Action Effects.

- Step 14 : To give action and see Inrerativities 1st by clicking on job classification as "White Collar" from Treemap Visual and data changes according selected field.

 
 ![ReportBookMark](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/d5f88c5c-6716-45e2-b712-8e999f746e1a)

  
 - Step 16 : To make Dashboard more interactive using filters. To do so selected the one visual for which we want to change the data according to it. After selecting click on Format tab and the select Edit Interation option on left top corner.

  Differnt sysmbols will apper on each visual at top right except the we one selected. We will select Highlight for "Balance Distribution" and  Filter for "New Customer By Months"

 ![image](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/f5eb0ba2-f2ea-4a4c-859f-de9d0d5aaedb)


# Making BI Visuals Inrerative using filters  (Power BI DESKTOP)

 
![BI_Interactivity](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/5d4f07df-321a-49ef-a4cc-900216ca0f1b)


- Step 16 : The report was then published to Power BI Service.
 
 
![PublishBI](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/a6e5ba97-8ee2-490d-85c3-4d1d8ef36e28)

# Snapshot of Dashboard (Power BI Service)

![image](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/3eae4147-c182-4039-8fa9-a21f3d07de18)


# Insights

A single page report was created on Power BI Desktop & it was then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Total Number of Customers = 4014

 Percentage of Customers with Job-Classification as white collar (Male+Femal) = 48.70 %

   Percentage of Customers with Job-Classification as Blue Collar (Male+Femal) = 26.13 %

Percentage of Customers with Job-Classification as other (Male+Femal) = 25.16 %
   


 thus, higher number of customers are of WHite Collar Job.
           

 ### [4] Some other insights

 
 ### Total number of custmers depending on age range:
    
    Age  group of 15 have total number of customer =54
    Age  group of 20 have total number of customer =182
    Age  group of 25 have total number of customer =482
    Age  group of 30 have total number of customer =801
    Age  group of 35 have total number of customer =797
    Age  group of 40 have total number of customer =616
    Age  group of 45 have total number of customer =452
    Age  group of 50 have total number of customer =332
    Age  group of 55 have total number of customer =202
    Age  group of 60 have total number of customer =96


 
  thus, maximum customers are of age 30-35 by Age Distribution.
 
 ### Balance Group by Customer ID
 
 2.1)  636 customers have 00.00 as their Bank Balance.
 
 2.2)  599 customers have 10000 as their Bank Balance.
 
 2.3)  581 customers have 20000 as their Bank Balance.
 
 2.4)  500 customers have 30000 as their Bank Balance.
 
 2.5)  420 customers have 40000 as their Bank Balance.

 2.6)  12 customers have 1,40,0000 as their Bank Balance.

 2.7)  2 customers have 1,80,000 as their Bank Balance. 

 2.8)  1 customer have 1,70,000 as Bank Balance. .

 2.9)  1 customer have 1,60,000 as Bank Balance.    
 
 thus, maximum customers belong to Zero Balance Account.
         
### Customer Type by Gender

3.1) 46.06 % i.e. 1849 customers have Customer Gender type 'Female'.

3.2) 53.94 % i.e. 2165 Customers have Customer Gender type 'Male'.
       
       thus, more customers have customer Male.

# SM Bank-Dashboard.md.txt
Displaying # SM Bank-Dashboard.md.txt.

![SM-Bank-DashBoard](https://github.com/SamruddhiMule/Project-for-Bank-Dashboard/assets/163804300/637fc22d-e54a-43d9-8215-70ae75934c42)















