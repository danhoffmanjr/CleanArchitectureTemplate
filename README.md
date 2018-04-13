# Clean Architecture Template
## How to use this template:
1. Download the CleanArchitecture.zip file
2. Create a new folder called Clean Architecture in the user project template directory for your version of Visual Studio. By default, this directory is %USERPROFILE%\Documents\Visual Studio <version>\Templates\ProjectTemplates.
3. Copy the CleanArchitecture.zip file into the Clean Architecture folder you created and unzip the file.
4. You should now see a Clean Architecture option under the Visual C# directory when you create a new project in Visual Studio.
  
## NOTE: Update the connection string in the appsettings.json file before running initial migrations for the database
There is one manual change you need to make to the appsettings.json file (in the App.Web project) to begin working with your SQL database. The connection string has placeholder elements in it by default. You need to manually replace the curley brace sections of the string, e.g., "aspnet-{REPLACE-WITH-PROJECT-NAME}-{REPLACE-WITH-GUID}" should be updated to something like "aspnet-BudgetManager-978265bb-0a60-4e62-8a6e-a20534331941" before running initial migrations and creating the database. 

To generate a new GUID for the connection string you can:
1. Use the built in GUID creator in Visual Studio (2017) under the Tools menu -> Create GUID -> use GUID format 4 (Registry format) and click NEW GUID and copy it.
2. Use an online GUID genertaor like https://guidgenerator.com/online-guid-generator.aspx

I hope this template is useful to you. Cheers!
