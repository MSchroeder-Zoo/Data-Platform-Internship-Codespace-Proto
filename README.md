# Data-Platform-Internship-Codespace-Proto 
Prototype Codespace for future DevOps at the stl zoo.

Start in the repo you would like the codespace to initlaize on.  
To launch codespace, select the green button labled "code" and manuver to the second tab labled "codespaces"  
Press the '+' button and initalize the codespace.  
Note: It may take a few minuets for the codespace to spin up.  

---

This codespace prototype contains most of the tools needed for DevOps work at the STL Zoo.  
### Tools included:  
- Powershell --> with AD modules installed
- Python 3.11 and various python addons (pylance, pip, jupyter, etc.)
- dbt
- ruff
- copilot
- wsl
- duckdb
- dagster
- docker
- dlt

---

The codespace tools can be modified at ./.devcontainer/devcontainer.json  
[GitHub devcontainer docs](https://docs.github.com/en/codespaces/setting-up-your-project-for-codespaces/configuring-dev-containers/adding-features-to-a-devcontainer-file)  

Once the codespace is launched in the browser, you can select the 3 horizonal lines in the top right corner to load the codespace in your local VS Code application.  
If you are using a free GH account, keep tabs on your codespace usage. Best practice is to not keep a codespace running if you are not activley using it. You can manage these settings in you GH profile settings under the "Usage" section.  
If you need to manually remove a codespace, navigate to the repository your codespace is located on and select the green button again. Click on the second tab and select the three dots above where your codespace is written.  
You should see an option to pause or delete the codespace. --> Note: If you delete a codespace without pushing changes to a branch, the changes will be deleted, this is not the case when pausing a codespace, such as when GH automatically does so, only for deletion.  


[GitHub has great documentation for using and customizing codespaces](https://docs.github.com/en/codespaces)  
These will be very helpful when needing to add, edit, or remove features to/from your codespace.  

---

When you have created your own repo for a project, copy and paste the contents of the devcontainer.json file in this repo into a file located at ./devcontainer/.devcontainer.json in your new repository before launching the codespace for the first time.  

### Other codespace notes:  
- for certain projects a .gitignore file will be needed. --> in this file place things that are not needed to be remade every time a codespace is created
  - Such as a .env file with an API key, database files, or pycache.
  - All you need to do for this is to add the file name that you would like to not persist:
     - .env *.duckdb datatable.csv, etc.
