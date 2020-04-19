# salesforceprofilemergetool

-> This is a tool made to automate various processes in org merge project.
-> In Org merge projects, there are requirements where there is need to combine 2 or more profiles into single profile and deploy that profile to the target org.
-> There was a requirement where final profile made by merging two or more profiles get the highest field permissions and the highest object permissions. 
-> Doing above process manually is time consuming, tidious and less accurate.
-> Hence, I developed this tool to automate this tidious process.


------- How To Use-----------------
1) Save code "profileMergeTool.vfp" and "profileComparitorCall.apxc" with same file name.
2) Update value of folder id in "profileComparitorCall.apxc" as per your salesforce org.
3) Run profileMergeTool.vfp
4) You will get picklist "SELECT PERMISSIONS"
5) "SELECT PERMISSIONS" has two values "objectPermissions" and "fieldPermissions"
6) Select any permission you want
7) Once you select permission, you will get two inputtext boxes. 1) "ENTER PROFILES TO BE MERGED" and 2) "ENTER OBJECTS TO BE COMPARED".
8) Enter all profiles to be merged with comma seperated value in "ENTER PROFILES TO BE MERGED" inputtext box and comma seperated object names in "ENTER OBJECTS TO BE COMPARED" inputtext box. 
9) Select "Generate" button.
10) Go to Document object in your Salesforce org.
11) You will find XML package of required permissions for target profile formed by merging profiles.
12) Deploy that package in target Salesforce org. 

Here is link of screencast to use this tool: https://www.screencast.com/t/CRdOuwBg2
