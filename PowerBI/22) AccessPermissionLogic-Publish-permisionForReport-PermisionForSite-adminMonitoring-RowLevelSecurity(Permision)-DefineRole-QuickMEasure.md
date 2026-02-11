# Session 22) AccessPermissionLogic-Publish-permisionForReport-PermisionForSite-adminMonitoring-RowLevelSecurity(Permision)-DefineRole-QuickMEasure

https://youtu.be/cjHC4eLO_cQ?si=MGPx5BaSnKYYrJER

# Access permission logic:
<img width="1394" height="229" alt="image" src="https://github.com/user-attachments/assets/5b97cedf-5c80-4f08-8583-87e2fde4791e" />
- Report Server Application > Manage Folder ⇒  we have a list of users and we can assign an access to them like:Browser (only view the report) , publish,..
- <img width="1393" height="817" alt="image" src="https://github.com/user-attachments/assets/222f0f5a-6905-4698-bafe-b7240d0e1e54" />
- We can also change the permission on each folder by click on “… “
- <img width="1240" height="490" alt="image" src="https://github.com/user-attachments/assets/1fb700b4-11b3-40e6-82a7-b73d4307e489" />

#  What is the logic of access permission?
## Ex: we have these folders and subfolders: 
  -<img width="736" height="134" alt="image" src="https://github.com/user-attachments/assets/663f0a45-9a21-488e-95c3-7e3010a15985" />
- Now we assign an access to users for each folder:
- Here we give the permission for Folder A to Khoobai and Hasnai ⇒So they also have access to subfolders.
- <img width="788" height="87" alt="image" src="https://github.com/user-attachments/assets/8a43842d-f958-40fb-9817-e20d0d3bcb66" />
-khoobai/hasani  have access to ⇒ a,b,c,d ,its sub folders
- Karimi  have access to ⇒only D and its subfolders
- Now we do the change in D folder
- <img width="835" height="98" alt="image" src="https://github.com/user-attachments/assets/f772c2f6-6095-486e-9dc0-c172a345591f" />
- Mohammadi is new user and we give the access permission for A folder
<img width="886" height="140" alt="image" src="https://github.com/user-attachments/assets/805099bf-246d-41c7-b93b-577d4843b572" />
<img width="853" height="96" alt="image" src="https://github.com/user-attachments/assets/99b85252-519c-4586-afbf-ce18986ffb1e" />

- When we see this Option in Security menu: <img width="264" height="122" alt="image" src="https://github.com/user-attachments/assets/50793e9b-32f0-488d-8b3f-8e9c3973a494" />
  - ⇒ it means ⇒ we manipulated  the folder and we have to give the direct permission for this folder to new user:
  - <img width="946" height="404" alt="image" src="https://github.com/user-attachments/assets/1758b5e4-4816-4f67-9477-d92fe5795b8c" />
- But if we  see <img width="265" height="117" alt="image" src="https://github.com/user-attachments/assets/cf52c648-706e-4632-bc7b-da38c62f6288" /> :
- <img width="822" height="486" alt="image" src="https://github.com/user-attachments/assets/fe339047-63ce-4638-9554-6f916061c39b" />
- <img width="712" height="75" alt="image" src="https://github.com/user-attachments/assets/5359da16-933c-4869-a621-b117022a0ba1" />


# Publish:
- We have to use  Power BI RS version ⇒ Power BI Report Server
There are 2 ways:
1) Save as>
- <img width="942" height="404" alt="image" src="https://github.com/user-attachments/assets/9b13b240-1374-4b2c-a658-d688e86f95a6" />
- Browse ⇒ save on our system
- Power BI Report Server ⇒ we can publish on  Report Server
    - Report Server application > copy URL:
    - <img width="574" height="325" alt="image" src="https://github.com/user-attachments/assets/184492ad-7bfd-4116-bfe7-b7326d0a8f32" />
    - Paste here (in powerbi> save as> powerbi report server):
    - <img width="680" height="463" alt="image" src="https://github.com/user-attachments/assets/59e4f08a-8116-4801-8055-8f90c1b4f366" />
<img width="830" height="64" alt="image" src="https://github.com/user-attachments/assets/b273863b-37a1-44ee-8d6b-d0906c995e0f" />
<img width="676" height="454" alt="image" src="https://github.com/user-attachments/assets/541c5a23-bdec-4948-8881-aed37f4c2ceb" />
- Select ShareReports:
- <img width="803" height="434" alt="image" src="https://github.com/user-attachments/assets/797eacdd-c163-4ac3-a20c-57d20ef43f87" />
- Now, if we go to Report server application , we can see our Reports

2) Report Server app > Upload button:
<img width="1585" height="367" alt="image" src="https://github.com/user-attachments/assets/c777f4b0-8080-4195-ad9e-5c72311650f8" />

<img width="1345" height="59" alt="image" src="https://github.com/user-attachments/assets/96cf5ebc-fd14-4c31-8ec0-0e0e7deae879" />

#  in Developer version:
<img width="1710" height="735" alt="image" src="https://github.com/user-attachments/assets/1199d000-3128-4e4d-ba50-49944eb0cb5a" />'

<img width="1625" height="148" alt="image" src="https://github.com/user-attachments/assets/d2e30532-7bc0-4240-ad8b-ab84201b835e" />


# Administration and monitoring the Pbix files:
- There is a pre define Dashboard that show how many visitor we had so far:
- <img width="931" height="623" alt="image" src="https://github.com/user-attachments/assets/63a29a0c-3ac8-4b7d-9988-3c6f5add407a" />
<img width="952" height="468" alt="image" src="https://github.com/user-attachments/assets/801f0618-6b3c-4157-80ad-d00fd00665e2" />
- We have connect this dashboard to our Data source that we have defined in report server.
- How to download:
  - <img width="726" height="52" alt="image" src="https://github.com/user-attachments/assets/ecaa2578-6bc6-466c-b6f4-4bc689373cc4" />
  - <img width="753" height="152" alt="image" src="https://github.com/user-attachments/assets/b76e0fd2-641c-4d75-9ea7-f1106ab91d8a" />
  - Then we have to find this dashboard (Pbix file)and download and use that for monitoring

# Row level security (RLS):
<img width="782" height="378" alt="image" src="https://github.com/user-attachments/assets/34318955-a272-428b-bdd6-cbd6b09dfb33" />
- define different Level of  access to different user
- in default, this menu id disable⇒ we have to create different Role  in PowerBI :
- Modeling >
-  ## manage Role
- <img width="796" height="175" alt="image" src="https://github.com/user-attachments/assets/e02c88ce-a1a8-4a78-91f4-47615a318748" />
<img width="788" height="467" alt="image" src="https://github.com/user-attachments/assets/79e9373d-57b9-4ca8-bcc5-8d62664b584e" />
- For example this is old version but this say ⇒ company B only see the Sales from Company A (R.K on table>Filter):
- Then click on <img width="274" height="126" alt="image" src="https://github.com/user-attachments/assets/ac6ca118-c784-4421-b503-1e3317f866ee" /> > Save
- Then publish again our dashboard to ReportServer > R.K on the dashboard name > manage > Row Level Security.
- now, if we open Report server ⇒ it doesn’t show us any dashboards , because we didn’t define Role for us:
- <img width="797" height="303" alt="image" src="https://github.com/user-attachments/assets/f28fbff7-76fe-41d1-b96f-cc8f798e1e0c" />
-  that’s a time to define Role in Report Server:
-  R.K on folder that contains our dashboard> manage > Row-Level-Security :
-  <img width="682" height="403" alt="image" src="https://github.com/user-attachments/assets/3b5ed0f2-15c6-487f-b210-68ffed1ff08a" />
- Add Member > write our ID or name and select their Role:
- <img width="776" height="413" alt="image" src="https://github.com/user-attachments/assets/96fac4a0-3536-408c-853b-229ea9bd2c16" />
- Like:
- <img width="565" height="312" alt="image" src="https://github.com/user-attachments/assets/dc178a17-1f98-4229-869e-71e10443e2e7" />
- Khoobani is subset of Company A , and each access tat company has ,Khobani also has.
- <img width="656" height="95" alt="image" src="https://github.com/user-attachments/assets/10b22881-782a-49e6-8fe9-2950570227b1" />
<img width="767" height="490" alt="image" src="https://github.com/user-attachments/assets/3b5d2125-d184-4756-9a58-bf1ddc817923" />

- ## With View As ⇒
- we can see the the result of access for each role in powerbi:
- <img width="814" height="194" alt="image" src="https://github.com/user-attachments/assets/6310f986-f012-4c3c-bce6-a8d4f8785abb" />
<img width="415" height="416" alt="image" src="https://github.com/user-attachments/assets/9e808537-6ac1-4f4a-8c9e-301f67bc3002" />

# Quick Measure:
<img width="603" height="257" alt="image" src="https://github.com/user-attachments/assets/322ed065-fef2-45ba-9919-cf2227d0f023" />
- Select  a predefined measure:
- <img width="570" height="797" alt="image" src="https://github.com/user-attachments/assets/a3866b6f-6a49-49ab-b236-7da8ff399374" />
- ex:
- <img width="791" height="822" alt="image" src="https://github.com/user-attachments/assets/019b24e3-80f6-46b3-8ffa-52d2eb420f28" />
- For example we create a quick measure on Base Value= CountPro column and doesn’t filter based on Category=Customer Name



