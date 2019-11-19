# git.for.MS.VS.Code
Git integration with Microsoft Visual code.

> Download Git and add install it.
> Command to check git version installed is ``` git --version ```
> For using git  for first time we need to configure email and git user name

### Configuring email and name on first log in to git
```
- git config --global user.email "Your Email Id"
- git config --global user.name "Your Name"
```
### Loading a folder to git version control
- Create a folder >> Open commond prompt or git bash
- Navigate to the folder location
- Run the command ``` git init ``` to add a folder to version control.

### Below spets are performed using Microsoft Visual Code
- Open the folder on MS code and follow the below steps.

### To Load project into Git Local Repository.
- Goto SCM (Source Control) icon and click on '+' symbol or initalize Repository
- it will show all the files in folder with 'U' which is untracked files
- to add this files to source control we need to commit them
- Commit this changes by clicking the "✓" symbol and add a messsage on the changes you made.
- Once Inital commit is sucessful you will not see anything in the SCM tab

### Modifying an existing files
- On changes any file from the project and saving, git will tract it, it will appear in SCM tab
- 'M' besides file in the SCM tab stands for modified
- You can stage this changes or undo this changes.
- Stage will let the file changes go into the next commit
- Undo will discard the changes
- You can see the changes made to a file by double clicking the file in SCM tab. (Opens the comparision tab)

### Undo the last commit if you accidentally commit something
- Switch to SCM tab, Click on the more options (three dots), choose undo last commit.

### Adding a remote repository for the same project and pushing code to it
- Goto Github.com and login create a new repository
- For adding an existing local repository to remote repository follow the below commands.
    - git remote add origin <<your repository link>>
    - git push -u origin master 
    example: git remote add origin https://github.com/Dhruvaraju/git.for.MS.VS.Code.git
    git push -u origin master

### Sometimes already existing repo cannot be merged with a local repository then use below
- git pull --allow-unrelated-histories <<repository url>>

### Updating local changes with remote repository
- Once you comple your changes in file save file commit the same
- goto SCM tab >> additional options '...' >> push this will publish your changes to remote repository
- you can all click the '🗘' synchronize changes in the status bar after code commit.
- while code sync is happening we will see a small clock icon on in the SCM tab icon

> For more descriptions on symbols as text search for unicode symbols
