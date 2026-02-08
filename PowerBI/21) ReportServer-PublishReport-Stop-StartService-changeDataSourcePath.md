# Session 21)ReportServer-PublishReport-Stop-Start Service-changeDataSourcePath

- https://youtu.be/6P539N_X4mY?si=Yyhy_mImt3tA6ZnR

- We use Report server to Publish our Report to use by clients

# Download Report Server Application:
https://www.microsoft.com/en-us/download/details.aspx?id=105944
<img width="696" height="488" alt="image" src="https://github.com/user-attachments/assets/b1b509fb-d8b4-4b3a-97ab-f876487b35da" />
- Select PowerBIReportServer:
- <img width="723" height="439" alt="image" src="https://github.com/user-attachments/assets/93177a5e-f764-4efa-a187-dce5c44cfd1f" />
- Install > select Developer in the menu:
- <img width="677" height="566" alt="image" src="https://github.com/user-attachments/assets/64d52e1c-a8f9-43eb-92b8-1b820d7c94b4" />
<img width="676" height="59" alt="image" src="https://github.com/user-attachments/assets/16e5cdac-2b00-4c80-9db1-083af332215d" />
- Now we need to configure Report Server and connect it to our server:
- <img width="663" height="508" alt="image" src="https://github.com/user-attachments/assets/7b9f0c0f-97af-45f1-b7ba-3a30434acbc4" />
- If we work on our laptop⇒ we connect to our server ex: RaziLaptop 
- else, if we want to connect to the specific Server ⇒ we have to write Server IP 
- Click on Connect button
- We can Stop or Start the service that run Report server in this part.
  - If we see the error on the report (in the future) ⇒ the server is stoped, we can come here and start it again
<img width="806" height="618" alt="image" src="https://github.com/user-attachments/assets/455b65db-5cb0-4ac6-8af4-1bf7c5c43380" />
- Now, we determine , who can connect to report server ans see the dashboard:
  - Network Service: al of the user in our same network can connect to our report server with their User and password
  - Virtual Service Account: only the user who have user ID of Report server can connect and see our report
  - <img width="591" height="104" alt="image" src="https://github.com/user-attachments/assets/08851aa6-8010-4220-a9de-6d7b80a1005e" />
  - Use another account: we can create an account for user who is in our network
  - <img width="413" height="33" alt="image" src="https://github.com/user-attachments/assets/755b670b-833a-40ba-8e0e-736412983c70" />
  <img width="801" height="664" alt="image" src="https://github.com/user-attachments/assets/988fb983-0626-4c88-a95c-1a5ff1718d63" />
  -  Apply ⇒ to save configurations
  -  Now, we can setup the directory name/ip address/port of Link  that client want to connect tour dashboard via that link:
  -    <img width="693" height="90" alt="image" src="https://github.com/user-attachments/assets/786faa41-c14e-4217-80e1-e407208a77f7" />
  - The best setting is  below  setting (but if the port was closed you can ask of network team and change the port)
  - <img width="827" height="408" alt="image" src="https://github.com/user-attachments/assets/7e31efca-8e93-4411-9737-6a591895ee13" />
  - We Can define  where  save all of the changes related to our dashboards which in on the report server:
  - <img width="814" height="384" alt="image" src="https://github.com/user-attachments/assets/b3e7d6f6-b70f-4607-a30e-4bbb2e75f769" />
  - Click on Change Database >
  - <img width="808" height="690" alt="image" src="https://github.com/user-attachments/assets/7dbdb770-617a-408d-a4f8-4a49cf5c2c06" />
  - <img width="775" height="402" alt="image" src="https://github.com/user-attachments/assets/2bcbdc8c-632a-4383-9db2-bc4e20a56f53" />
- Create database in current user (our laptop) or another server ⇒ I selected current user > Test connection
- Next
- <img width="553" height="137" alt="image" src="https://github.com/user-attachments/assets/36e749da-b00e-4e0b-bf95-b3b6b537b72e" />
- Select type:
- <img width="774" height="223" alt="image" src="https://github.com/user-attachments/assets/72b8ccc1-9cea-4aa2-abb9-e416b573af91" />
- Next > finish
- This is final step and we want set the URL name that user want use that:
- <img width="868" height="180" alt="image" src="https://github.com/user-attachments/assets/0e88c879-e672-4f0c-a198-8bbc82eeb017" />
- In Virtual Directory⇒ we write the name that want add at the end of the URL link.

# Upload our Dashboard on the Report Server that we created:
<img width="1191" height="138" alt="image" src="https://github.com/user-attachments/assets/e2635070-f628-4cb3-b5b4-ce43821aaf7f" />
- When the dashboard is published, some options become available:
- <img width="1194" height="276" alt="image" src="https://github.com/user-attachments/assets/67b14810-0f46-4405-bf19-2dc729ebc271" />
- We can organise with creating  Folder
- Each dashboard has some options like: add to favorite,..
- <img width="903" height="590" alt="image" src="https://github.com/user-attachments/assets/4d6d45fa-e006-421d-b541-6b4089450bb0" />
  - Manage option:
  - Properties⇒ Rename dashboard name / hide or unhide
  - <img width="1111" height="705" alt="image" src="https://github.com/user-attachments/assets/527fa410-f5aa-4709-a333-9b6578121f57" />
  - Scheduled Update: Determine when this dashboard will update.
  - <img width="1132" height="273" alt="image" src="https://github.com/user-attachments/assets/32824d86-4b0b-4354-99f4-b3afa8943f23" />
  - Set editing time ⇒ Edit >
  - <img width="709" height="376" alt="image" src="https://github.com/user-attachments/assets/e15429b0-6846-417c-9ac3-68b917fc5f7e" />
  - Edit schedule: set the update time > Apply
  - <img width="623" height="681" alt="image" src="https://github.com/user-attachments/assets/e7391238-e19b-4036-a072-12e710333276" />
  <img width="792" height="114" alt="image" src="https://github.com/user-attachments/assets/6400260f-2699-4e77-a7db-b8d2f85b3422" />
  - # Define the Data source path for this dashboard:
  - <img width="837" height="724" alt="image" src="https://github.com/user-attachments/assets/534c596e-2493-4332-bc06-6983ca4a2730" />
  - Connection String ⇒ is Data source Path
  - Authentication Type ⇒ determine the type of access to  data source
  - For example for SQL we set the data base name  in Basic authentication , write user password > ok
  - <img width="559" height="569" alt="image" src="https://github.com/user-attachments/assets/73ca4561-4d24-48f9-a2a2-abe91c8dde80" />
-   But for Excel we have to be careful:
- We have to insert Dynamic Address ,not static.
- This below address is dynamic and doesn’t give us an error:
- <img width="618" height="554" alt="image" src="https://github.com/user-attachments/assets/b567668e-c07b-414d-b3fe-1cd42a56812a" />
- But this one is staticaddress and  give us an error:
- <img width="734" height="699" alt="image" src="https://github.com/user-attachments/assets/392ea82b-1f75-4f6c-aa15-56de688531df" />
<img width="539" height="200" alt="image" src="https://github.com/user-attachments/assets/371af986-c0f9-4175-b867-c0a363b2aced" />
- We have to share the folder who is contain the dashboard and we have to give access to each user:
- No we can use the address that start with\\Share\..
- <img width="460" height="109" alt="image" src="https://github.com/user-attachments/assets/68a8f7a4-23b4-4af9-bc18-0a826c8fa047" />
<img width="1085" height="700" alt="image" src="https://github.com/user-attachments/assets/2010a560-1cd6-4a65-a272-b345bb3b25a4" />

# Change Data source that contain Excel file:
- Share the folder which contain the excel file in windows
- Make path static address ⇒ to dynamic address:
- <img width="675" height="319" alt="image" src="https://github.com/user-attachments/assets/042c8203-777c-47ae-ab98-4e5ceaade8cb" />

## Change source  (change data Source path)> write dynamic address  which start with //share-foldername (because in company there is onle one share folder) or //laptop-name/..:
<img width="972" height="712" alt="image" src="https://github.com/user-attachments/assets/abe21936-33ef-4ad1-8148-ceab01452c9c" />
<img width="1143" height="394" alt="image" src="https://github.com/user-attachments/assets/6bd44827-4367-41ab-9771-47e3015a9ed6" />
- For example ⇒ \\Khobani-laptob\d\personal…\file.xlsx
- Note: if we want to make sure the share folder is correct:
- Write  this line id address bar of folder in windows⇒ 
<img width="200" height="64" alt="image" src="https://github.com/user-attachments/assets/ca79fb03-289a-448b-b2ba-27c405e38d6d" />

<img width="460" height="433" alt="image" src="https://github.com/user-attachments/assets/cf37f36a-e89a-4c22-8c2c-5b32e1ab9f19" />

















  

















