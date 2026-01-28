# Session 15: DAXconcept-ImportantWebsite-percentage-FilterInPowerBI-Menu

- https://youtu.be/s9lEVyoAP78?si=p_ntBtBske2GoCth
# These are 2 important website that we can learn about DAX():
- https://learn.microsoft.com/en-us/dax/
- https://dax.guide/

#  Other important website:
- https://www.sqlbi.com/
- https://okviz.com/our-visuals/ ⇒ we can download different Visual for our Dashboard
- https://dax.do/ ⇒ there is a sample table and virtual environment to code ,run  the DAX codes
- https://www.daxpatterns.com/ ⇒ we can download Dax book / also we can learn the spacial Analysis like Ranking , Basket analysis and ..
- https://www.daxformatter.com/ ⇒ make your DAX code easy to read and give us a good format
- https://bravo.bi/ ⇒ Use Bravo to quickly analyze where your model consumes the most memory and choose which columns to remove to optimize it. You can also use Bravo to export your metadata to VPAX files.

#  Essential BI Tools: 
- https://www.sqlbi.com/tools/
- <img width="651" height="547" alt="image" src="https://github.com/user-attachments/assets/794e0c4f-ece8-4629-b030-d5b5171623b2" />
<img width="403" height="401" alt="image" src="https://github.com/user-attachments/assets/a1abaad3-ab78-4c1d-addb-7c1a76ab4934" />
- We can optimize our table with this tool (later we will realize that there is a column that we are not using, so we use this tool to optimize it)
<img width="379" height="380" alt="image" src="https://github.com/user-attachments/assets/d15f53b9-313e-4c2a-b65f-38d84336d160" />
- We write our code in this tools, it clean code and check performance
- Dax ⇒ is a language for make relation with data

# Application of DAX:
- powerBI > select table in Data tab > tools menu:
- <img width="755" height="292" alt="image" src="https://github.com/user-attachments/assets/169fb1a6-06c2-4b25-8a42-c7266119c5ce" />
- Create Measure (new measure)
  - Output is always ⇒ a number (we can’t have a column as an output)
  - Quick measure ⇒ it’s with wizard (quick)
- Create Column (new column)
  - Output is always ⇒ a Column
- Create Table (New Table)
  - Output is always ⇒ a table


# Functions in DAX:
- https://dax.guide/
<img width="888" height="430" alt="image" src="https://github.com/user-attachments/assets/7e351f00-6366-4088-adaf-7bc860f794cc" />
- We have different Category functions:
- Aggregation function:
  - Sum / groupby / join /summerize/..
- Date & Time function
- Filter function
- Logical function
- Math and trig function
- Parent-child functions
- Relationships management functions
- Table manipulation functions
- Text functions

# Note:showing the Percentage 
- When we want show the percentage of the value to total , in our visual:
- Select visual like bar chart > Visualization > x or y-axis >
- <img width="765" height="673" alt="image" src="https://github.com/user-attachments/assets/c2dae37e-733b-4f6f-bf98-940a826868ab" />
- Show value as > Percent of grand total:
- <img width="604" height="683" alt="image" src="https://github.com/user-attachments/assets/0b5716bd-136b-42b4-955c-d382b7c38652" />
<img width="567" height="403" alt="image" src="https://github.com/user-attachments/assets/6bcb043c-c28b-41cc-8b12-5937b9ab17a7" />
#  we have  different kinds of Percentage:
<img width="502" height="169" alt="image" src="https://github.com/user-attachments/assets/a5bd1fd0-8185-4cc5-8a63-a97ea9614fbd" />
<img width="753" height="334" alt="image" src="https://github.com/user-attachments/assets/8a57d721-4fc3-4c9f-a222-315d2176a6dc" />
- Percent of grand total
  -  Calculates the percentage of each value relative to the total of the entire table.
  -  <img width="422" height="304" alt="image" src="https://github.com/user-attachments/assets/08f1d3db-82a5-4291-a7ac-49c815ec9d4c" />
- Percent of column total
  - Calculates the percentage of each value relative to the total of its column.
  - <img width="438" height="308" alt="image" src="https://github.com/user-attachments/assets/cd3ed56a-8f58-48ac-ab4a-48c80dadb2d9" />
- Percent of row total
   - Calculates the percentage of each value relative to the total of its row.
   - <img width="405" height="320" alt="image" src="https://github.com/user-attachments/assets/dbe34ff7-73f5-4769-9ab6-a6c4603633c6" />

# Dax:
- # New Column:
  - powerBI >  Table view
  - <img width="267" height="417" alt="image" src="https://github.com/user-attachments/assets/110d9840-9dad-4ae0-b03d-ac85bd578965" />
  - Table Tools menu >New column
  - <img width="646" height="464" alt="image" src="https://github.com/user-attachments/assets/63b28201-08ea-4a43-a9d9-876624419715" />
  - To write a DAX code:
    - We have to assign a name to each line code:
    - <img width="838" height="213" alt="image" src="https://github.com/user-attachments/assets/dbb84b1c-ebbf-4c79-a047-5dce85403d23" />
    - Like:
    - <img width="749" height="390" alt="image" src="https://github.com/user-attachments/assets/a163edb3-44ea-4baa-bbb2-6f865ed0785f" />
- # Note:  When there is a relationship between two tables, Power BI treats them as a single table.
- In below example Calender can filter the Sales table but sales can’t filter calender table
- <img width="654" height="318" alt="image" src="https://github.com/user-attachments/assets/84ffd323-4fc4-46ec-a83d-68f41c0e5bbf" />
- # Sum function ⇒
  -  without applying Filtering (they don’t consider the relation between tables , they only Summarise all of the data )
  -  <img width="843" height="202" alt="image" src="https://github.com/user-attachments/assets/bd0b9180-d2fc-4ed9-90e4-778ae5f0a44f" />
- # Calculate()==>
-   <img width="790" height="85" alt="image" src="https://github.com/user-attachments/assets/ddff96bb-fdac-4ae7-b057-af30a1a66ff6" />
<img width="618" height="142" alt="image" src="https://github.com/user-attachments/assets/6dac8849-65ad-4b3e-858d-a58af353e5e7" />

# Ex:Filter the Chart  in Power BI:
  - Show 5 Top Person  based on their Revenue
  - <img width="856" height="487" alt="image" src="https://github.com/user-attachments/assets/fe2e3251-185b-4d0e-a33f-d2aebb38f355" />

#  Note: 
- ex: <img width="843" height="70" alt="image" src="https://github.com/user-attachments/assets/35ef06e9-6113-4ddf-8340-e7cfc7ad2c2d" />

- Design a main dashboard in page 1
- <img width="856" height="398" alt="image" src="https://github.com/user-attachments/assets/b1166771-cda9-4539-84db-45bb3879e9bd" />
- Make a copy of page 1 then using photoshop, powerpoint or.. Edit the visual of page 1  ⇒ and - paste in page 2 ⇒ r.k on page 2 name > Hide
- <img width="703" height="393" alt="image" src="https://github.com/user-attachments/assets/57d67f00-c6ee-45ea-99c5-895e4285530c" />
- Insert a button or shape in page 1 > Action = Page navigator > select page 2
- Now, we are able to to create Menu  without Bookmark










  





    

    


  


  


   


  









