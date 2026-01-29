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
- # New Measure:
   - Power BI > Data panel > on the desired table > R.K > new measure
   - <img width="523" height="540" alt="image" src="https://github.com/user-attachments/assets/5ac62ecf-5728-4e6c-b285-63edffaed9bd" />

   - <img width="465" height="74" alt="image" src="https://github.com/user-attachments/assets/3ae49ba5-845c-4f7b-a552-26e8c1b03824" />
   - Enter > new column (sum Revenue) added to our table
   - <img width="205" height="490" alt="image" src="https://github.com/user-attachments/assets/e36ba166-fa06-4c29-b25f-c40b19b42b10" />
   - Now we can use this column to plot chart:
   - <img width="322" height="558" alt="image" src="https://github.com/user-attachments/assets/b75633be-ae1f-457d-9e68-0d5bb07f9cce" />
   <img width="453" height="364" alt="image" src="https://github.com/user-attachments/assets/1ad4ff43-ad88-40cb-adfa-f53246725e1e" />

- # Average:
- <img width="502" height="154" alt="image" src="https://github.com/user-attachments/assets/553f4e50-dc02-44cf-becd-9e2bddd7808c" />
 - We can set some setting for our dax output:
 - For example : while number or number of decimal
 - <img width="619" height="255" alt="image" src="https://github.com/user-attachments/assets/b8bbfa22-a902-4ff3-8a20-ab40bee2ceb6" />
 - if we put Average as x with category as y axis  in one chart, it will be filter the average(x) based on filters
 - <img width="522" height="425" alt="image" src="https://github.com/user-attachments/assets/1f7151d9-4a8c-46e1-ad93-acf5fab09892" />
 
- # Count:
- <img width="523" height="54" alt="image" src="https://github.com/user-attachments/assets/ec70d7f2-0fd6-4103-a77e-eb083840e45c" />

- # DistinctCount() 
   - Count Number of unique values
   - <img width="358" height="45" alt="image" src="https://github.com/user-attachments/assets/6b3257f6-5cb5-4da3-bea2-1e69351ed228" />
  
- # Countrows()
   -  Count Null value
   -  <img width="307" height="43" alt="image" src="https://github.com/user-attachments/assets/116b0a5e-199f-453d-9966-709257c7a2a1" />
   
- # countblank()
-  # Comment :
   - To make comment one lines :
   - <img width="380" height="87" alt="image" src="https://github.com/user-attachments/assets/fb9eeac8-aab5-41c9-99ad-5d13de3b50f0" />
   - To comment multiple lines:
   - <img width="379" height="71" alt="image" src="https://github.com/user-attachments/assets/2afcfade-f2d9-45d5-af99-ddd09e1c84be" />
   
- # calculate:
  -  When we want write a code that consider filter we use  this:
  -  <img width="400" height="195" alt="image" src="https://github.com/user-attachments/assets/6e805628-d152-4bfd-bfb2-d4514ac25111" />
  - Expression ⇒ is any code like sum,count,..
  - Filter ⇒ write a condition or filter  like : tblsales[Category] <> “oil”
  - <img width="619" height="54" alt="image" src="https://github.com/user-attachments/assets/ce7fd153-6d2c-4356-86ec-563024032717" />
  - Sum the revenue for  all of the categories ,except “oil”
  - <img width="651" height="51" alt="image" src="https://github.com/user-attachments/assets/19ee70da-0c36-4338-83ba-edb07cd4dfd0" />
  - Sum the revenue of only oil category

  


Sum the revenue of only oil category

