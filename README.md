# HR-Analytics-Dashboard

## Dashboard Link: https://app.powerbi.com/groups/me/reports/e7d657d0-9790-4f7a-ba40-39be6870571e/f6c7ed71e1c108aaab7d?experience=power-bi

## Process for preparing the project:

A.Understanding Business requirement: The report has been created keeping in mind the following question from the Clients End:

1) How many people are in each job?
2) Gender break-down of the staff
3) Age spread of the staff
4) Which jobs pay more?
5) Top earners in each job
6) Qualification vs. Salary
7) Staff growth trend over time
8) Employee filter by starting letter
9) Leave balance analysis
10) Quick HR Dashboard

B.Data Walkthrough: The Data was preety precise and contained no null values or duplicate values.

#### ❖	Overview : 
The dataset contains feature vectors for 161 data points. The data is curated to avoid bias in order to derive genuine results. The dataset consists of a total of 8 columns out of which - 4 contain string data type, 1 date column and 3 mumerical attributes.

#### ❖	Explanation: 
The dataset includes the following fields:

●	Emp ID : Unique Value given to employees for identification.

●	Gender: Gender of the employees.

● Educational Qualification : Educational Background of the employee.

●	Date of Join: The date when the employee joined the organisation.

●	Job Title : Type of work designation of the employee.

●	Salary : Salary p.a of the employee

●	Age : No of years on Earth.

●	Leave Balance : amount of leave (such as paid time off, sick leave, vacation days, etc.) that an employee has accumulated or is entitled to use but has not yet used.

### ❖ Steps followed 

- Step 1 : Load dataset into Power BI Desktop, dataset is an xlxs file type.
- Step 2 : Open power query editor & in view tab under Data preview section, check "column distribution", "column quality" & "column profile" options.
- Step 3 : Also since by default, profile will be opened only for 1000 rows so you need to select "column profiling based on entire dataset".
- Step 4 : It was observed that in none of the columns, errors & empty values and no duplicates.
- Step 5 : A new column with only the first characters of the name of the employees was created for use in report view.
- Step 6 : Four card visuals were added to the canvas, representing Total Employees, Avg of Salary, Avg Leave Balance, LBL.
- Step 7 : New measure were for the following calculations.
  Following DAX expression was written for the same,
  
 1. Total Employees = DISTINCTCOUNT(data[Emp ID])
    
   A card visual was used to represent this.
   
   Snap of Total Employees

  ![Screenshot 2024-12-20 223622](https://github.com/user-attachments/assets/15e325d7-b131-45a1-8b43-7a5fc0f89a03)

  2. Avg of Salary = AVERAGE(data[Salary])

   A card visual was used to represent this.
   
   Snap of Avg Salary

   ![Screenshot 2024-12-20 231104](https://github.com/user-attachments/assets/9a0c9344-16d4-4f9d-9b64-80b0a8c3635c)

  3. Avg Leave Balance = AVERAGE(data[Leave Balance])

    A card visual was used to represent this.
   
    Snap of Avg Leave Balance

  ![Screenshot 2024-12-20 231234](https://github.com/user-attachments/assets/e7a596f3-6593-4681-b679-019e91a41240)

  4. LBL = CALCULATE([Total Employees], data[Leave Balance] > 20)

    A card visual was used to represent this.
   
    Snap of LBL

  ![Screenshot 2024-12-20 231403](https://github.com/user-attachments/assets/48bb15c3-f911-433e-97d0-72fdfeef0a7b)


  #### Report Snapshot (Power BI DESKTOP) 

  Snap Of Home Page:

  ![Screenshot 2024-12-20 231636](https://github.com/user-attachments/assets/fef4ec00-d332-4c6f-9f9d-3eb9aef72404)

  Snap of Top Earners and Staff Growth Trend:

  ![Screenshot 2024-12-20 231717](https://github.com/user-attachments/assets/232a785b-fbcb-4488-b71f-c444c58cd056)

  Snap Of Employees Details:

  ![Screenshot 2024-12-20 231805](https://github.com/user-attachments/assets/1791fce9-a722-4027-b069-740e1c0c683a)

  Snap of HR Analytics Dashboard:

  ![Screenshot 2024-12-20 231543](https://github.com/user-attachments/assets/0c296dd8-417d-46c9-bcb3-c0a8b4f1ddbd)
    
     
