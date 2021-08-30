To run this bot you need to do some changes
1. Create Database and configure it into Connect activity
2. Create SPs 

CREATE PROCEDURE LeftJoin
AS
SELECT Department_Name, Name, Joining_Date FROM New_Joinings_Details LEFT JOIN Department_Details ON New_Joinings_Details.Department_id = Department_Details.Department_id;
GO;


Delete_New_Joinings

Delete New_Joinings_Details;

3. Input file path in Excel (step 5)

4. Retrived Data file pathy (step 14,22)

5. Master_Excel.xlsx file path (step 16)

6. Mail Details (step 38)

taible details

table name : Department_Details
	Columns Department_id nvarchar , Department_Name nvarchar
    
table name : New_Joinings_Details
	Columns Department_id nvarchar , Name nvarchar , Joining_Date nvarchar
    
   
