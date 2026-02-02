# Session 19)  - Dax-Calculate-LeftToRight-All(= remove filter)-Edit Interaction(visual Independence)-Variable-SelectedValue-IF-RadioButton-HasNoValue-YOY-MOM-GenerateSeries
https://youtu.be/0WauCkI1O9k?si=pweJDszTx9CLibvP

# Calculate:
- Read from Left to Right:
- <img width="887" height="302" alt="image" src="https://github.com/user-attachments/assets/5bea9c27-a7b3-434c-a708-3e9a5a6be6da" />
- First ⇒ sum(Revenue)  
- Then⇒ apply this filter (category=”ada”) on the result of first step =is like Slicer
- like:
- <img width="1374" height="699" alt="image" src="https://github.com/user-attachments/assets/9ae73933-2049-400a-99a2-5402e1972cde" />

# All:
- Is like Remove Filter based on X
- Like: in below measure we say⇒ sum(revenue) ⇒ then : if you see Category column, don’t filter by “Category” column
- <img width="1512" height="773" alt="image" src="https://github.com/user-attachments/assets/19d2da91-e3ad-46ae-96b8-18e5a4d14991" />

# EX: write a Dax code to show the Share Sale based of Year:
- <img width="854" height="381" alt="image" src="https://github.com/user-attachments/assets/72277167-3899-4231-8dd9-29aeecdb95db" />
- Answer:
- <img width="772" height="192" alt="image" src="https://github.com/user-attachments/assets/c7989fd6-3a4a-45da-9b94-1b43d9bcda45" />
- This code equal to : Percentage of grand total
- <img width="682" height="306" alt="image" src="https://github.com/user-attachments/assets/e1522c6d-0f98-49d7-8547-e1fe4da43afc" />
- <img width="1643" height="705" alt="image" src="https://github.com/user-attachments/assets/9ae1a3a8-55aa-4ccb-ae8c-3cb40427b7cb" />
- If I put Legend=Category ⇒ it shows my Visual for all categories
- <img width="1713" height="757" alt="image" src="https://github.com/user-attachments/assets/ef5c8af4-2ffe-4fa7-b618-3e20f58a1be5" />

# Edit interaction: 
- How to make two visuals independent in Power BI
- <img width="1212" height="586" alt="image" src="https://github.com/user-attachments/assets/f5b39285-54de-41a2-b2ea-74c37f000828" />
<img width="682" height="659" alt="image" src="https://github.com/user-attachments/assets/c2d07fb0-d88e-47d7-9cd7-ae01663788c0" />

# All Except:
- filter Only with this element
- <img width="1212" height="178" alt="image" src="https://github.com/user-attachments/assets/9d4767ae-e5b9-4a41-ba6a-a6c0ca71f3ae" />
- This measure will be filter only with Category field
- <img width="1570" height="612" alt="image" src="https://github.com/user-attachments/assets/0cd73f3a-bb0e-4e36-a3a2-b6853e525041" />
# AllNoBlankRow:
- Filter the table that doesn’t have NULL value
- <img width="759" height="167" alt="image" src="https://github.com/user-attachments/assets/6b60104e-b9f6-4bc9-9252-46b4a441a1bb" />

# AllSelected:
- Returns all the rows in a table, or all the values in a column, ignoring any filters that might have been applied inside the query, but keeping filters that come from outside.
- <img width="784" height="485" alt="image" src="https://github.com/user-attachments/assets/f536b120-e6f4-4475-be91-b5e6419131f7" />

# DAX Variable:
- Make Measure > using Var for define variable > using Return >  and final formula to return output, like:
- <img width="232" height="154" alt="image" src="https://github.com/user-attachments/assets/ad0e92bd-a362-429a-be5f-de70895ea4ef" />
- <img width="775" height="480" alt="image" src="https://github.com/user-attachments/assets/4e69e448-ec28-4db8-9f95-9bdf1f7ab547" />
- <img width="642" height="666" alt="image" src="https://github.com/user-attachments/assets/54aec90f-f95a-4a89-8833-9a76ee06fdd5" />
- <img width="599" height="632" alt="image" src="https://github.com/user-attachments/assets/38b65113-7d39-4f35-8d36-916330b43855" />
- <img width="644" height="340" alt="image" src="https://github.com/user-attachments/assets/e8223270-b96b-4bcc-9af3-98bb843fb4f8" />
- # Calculate only change Expression , not values
- <img width="629" height="357" alt="image" src="https://github.com/user-attachments/assets/6b67e273-c2e1-4c8b-890a-fd4c5a479181" />
- <img width="629" height="427" alt="image" src="https://github.com/user-attachments/assets/e86635b7-f64c-4d49-bac4-133cb3ba2da8" />
- # Return:
- <img width="616" height="453" alt="image" src="https://github.com/user-attachments/assets/c609866a-f65d-4f7f-afc0-91b01c71768c" />
- <img width="630" height="399" alt="image" src="https://github.com/user-attachments/assets/3399ce6b-a074-4f86-a8fc-67fd62e6d0d6" />

# GenerateSeries(from,to,step) using DAX:
- <img width="375" height="190" alt="image" src="https://github.com/user-attachments/assets/fa5f7f1c-6073-4283-8476-6efffb364fe3" />
- New Table >
- <img width="759" height="140" alt="image" src="https://github.com/user-attachments/assets/e52a157b-bc5b-4836-928d-afe82e91d4cc" />
- <img width="167" height="539" alt="image" src="https://github.com/user-attachments/assets/7c9fcefa-90a3-42d9-945e-7abb3d78615c" />

# SelectedValue  &  IF:
- To define default value for for example Slicer when we don’t select any option:
- <img width="1532" height="521" alt="image" src="https://github.com/user-attachments/assets/1615dc8a-82e4-4d1d-b55a-bc273cf7781e" />
- New Measure >
- <img width="651" height="74" alt="image" src="https://github.com/user-attachments/assets/eb98d431-2fb1-4f1e-ab6e-ef7164bfcc35" />
- Means ⇒ if (any visual like slicer ⇒ selected a year option) >  then show the year value > else show number one (1)
- Or we can write a text:
- <img width="809" height="111" alt="image" src="https://github.com/user-attachments/assets/8722d8db-9697-4a17-9d50-f6dc7b3688f6" />
- Now we want to write more professional with IF:
- <img width="783" height="278" alt="image" src="https://github.com/user-attachments/assets/c77e2f4e-ae52-40ae-a938-6bb869de91bd" />
- <img width="1716" height="685" alt="image" src="https://github.com/user-attachments/assets/b31743e9-44ba-4bd6-b75e-3b515eef67b4" />
- <img width="632" height="645" alt="image" src="https://github.com/user-attachments/assets/4a286989-456a-494a-b205-f97c8d53a0e6" />
- # Radio Button(single selection):
- If we want to only allow one option to be selected (like as a Radio button): enable ⇒ Single select
- <img width="551" height="624" alt="image" src="https://github.com/user-attachments/assets/8d082afe-c56c-46eb-8131-9e25cb1b0399" />
- Or  With DAX code:
-  # HasNoValue(ColumnName):
-  - <img width="412" height="190" alt="image" src="https://github.com/user-attachments/assets/feabba8a-d1d0-4778-80ec-7129f2d5a74d" />
- <img width="739" height="615" alt="image" src="https://github.com/user-attachments/assets/55bbf06f-6bda-4e37-8fe1-71ac363fd4ca" />

# Ex: Growth rate (YOY- MOM):
- We have this table:
- <img width="1453" height="563" alt="image" src="https://github.com/user-attachments/assets/db6d21db-9530-4b14-a76f-9f0daac3ce36" />
- 1) Now create a table that shows the ratio of each month's growth rate to the previous month (as Percentage format). 
  - Formula is ⇒ (current Sale - previous month sale) /  previous month sale
  - <img width="599" height="111" alt="image" src="https://github.com/user-attachments/assets/9b0d9b7d-1220-4dac-a96b-d5eb20c61844" />
- 2) create a Slicer for number 1 to 24:
  - If I select number 2 ⇒growth rate of ( this month - 2 month previous)
  - If 6 ⇒growth rate of ( this month - 6 month previous)
- 3) if there is positive growth /negative growth / nothing ⇒ shows icon:
     - <img width="1352" height="742" alt="image" src="https://github.com/user-attachments/assets/c1f1d2a8-00a4-47c7-89f0-8eed607ccfb7" />
     - <img width="863" height="623" alt="image" src="https://github.com/user-attachments/assets/1912c047-7a6a-4133-aa8c-f94bf4c170bf" />
 - For answer we can use Date functions like:
 - <img width="606" height="175" alt="image" src="https://github.com/user-attachments/assets/e4502c6d-40fe-40cf-9722-88f75f29c016" />
     















 





















- 




























