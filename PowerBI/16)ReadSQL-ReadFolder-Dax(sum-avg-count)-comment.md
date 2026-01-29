Session 16) ReadSQL-ReadFolder-Dax(sum-avg-count)-comment
https://youtu.be/VPTL2OoS-KA?si=CfNNR08h_jz_Xs7X
# Read from SQL:

Enter IP Server :
If I insert “.” dot ⇒ it means , read from the SQL which is on my system, 
Otherwise⇒ we have to enter IP Server
> OK
Enter Username & Password Of SQL > connect
# Note:  If we have MySQL or Oracle or.. : 
We have to install an application to connect PowerBI to our Datbase
For example we search:

Open ⇒


Now, we can get help of Microsoft website to connect to powerBI

# Read Folder of excel files (Combine) :
Home > Get Data > Folder > connect > select folder> ok> Combine & Load >
We define our sample that we want  combine all of the files in this format with these columns:

> select desired table> ok
Note: we can Change the Sample file later:

Now, if we add another file with this format (sample file) in this folder ⇒ Power Bi read the data automatically  and append to end of the files
If 2 tables don’t be the same ⇒ powerBI filled the column by Null Value:

But e can have a setting to append just a tables which has exactly the same columns


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

