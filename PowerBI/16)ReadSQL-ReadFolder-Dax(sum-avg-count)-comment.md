# Session 16) ReadSQL-ReadFolder-Dax(sum-avg-count)-comment
https://youtu.be/VPTL2OoS-KA?si=CfNNR08h_jz_Xs7X

# Read from SQL:
<img width="387" height="503" alt="image" src="https://github.com/user-attachments/assets/a1200c1f-f430-45d8-87b6-8d5ef53b7485" />
- Enter IP Server :
 - If I insert “.” dot ⇒ it means , read from the SQL which is on my system, 
 - Otherwise⇒ we have to enter IP Server
 - <img width="602" height="268" alt="image" src="https://github.com/user-attachments/assets/befcaa63-d81c-421d-a827-664dfa50da62" />
 - Enter Username & Password Of SQL > connect
 - # Note:  If we have MySQL or Oracle or.. : 
   - We have to install an application to connect PowerBI to our Datbase
   - For example we search:
   - <img width="631" height="514" alt="image" src="https://github.com/user-attachments/assets/53da712c-56a3-466b-a93a-309581892eb2" />
   - Open ⇒
   - <img width="500" height="173" alt="image" src="https://github.com/user-attachments/assets/21c4e773-f7dd-4756-bf51-94f2e77e3d29" />
   <img width="896" height="496" alt="image" src="https://github.com/user-attachments/assets/2fe36b11-9394-4c10-a39d-6dc8c663447b" />
   - Now, we can get help of Microsoft website to connect to powerBI


# Read Folder of excel files (Combine) :
- Home > Get Data > Folder > connect > select folder> ok>
- # Combine & Load >
- We define our sample that we want  combine all of the files in this format with these columns:
- <img width="667" height="526" alt="image" src="https://github.com/user-attachments/assets/47ed093f-eed4-46af-8cba-f985ae998a72" />
- > select desired table> ok
- Note: we can Change the Sample file later:
- <img width="749" height="558" alt="image" src="https://github.com/user-attachments/assets/683db704-4eba-4861-8361-577c7b465020" />
- If 2 tables don’t be the same ⇒ powerBI filled the column by Null Value:
- <img width="799" height="348" alt="image" src="https://github.com/user-attachments/assets/2eb146fd-c949-4c80-a281-f46ef20dfe54" />
- But e can have a setting to append just a tables which has exactly the same columns


# DAX:
# New Measure:
Power BI > Data panel > on the desired table > R.K > new measure


Enter > new column (sum Revenue) added to our table 

Now we can use this column to plot chart:


# Average:

We can set some setting for our dax output:
For example : while number or number of decimal



if we put Average as x with category as y axis  in one chart, it will be filter the average(x) based on filters

# Count: 

# DistinctCount() 
Count Number of unique values

# Countrows()
Count Null value

# countblank()


# Comment : 
To make comment one lines :
 
To comment multiple lines:


# calculate: 
When we want write a code that consider filter we use  this:

Expression ⇒ is any code like sum,count,..
Filter ⇒ write a condition or filter  like : tblsales[Category] <> “oil”

Sum the revenue for  all of the categories ,except “oil”

Sum the revenue of only oil category

