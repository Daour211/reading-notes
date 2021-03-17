## Version Control:


Version control: *is a system which allows to revert various versions of the file by recoding the changes*. And this allows me to revert to the file pervious version. There are three versions of VS:

- LVS
- CVS
- DVSC

Git is DVSC. It was created by Linux Torvalds. 

After installing Git a customizations steps need to be done. 

### Workflow:

Local Git repository has three components:

-Working Directory: actual files reside here.
-Index: area used for staging
-Head: points to the most recent commit

### Cloning: 

It is to create a copy of an existing repository from a server "GitHub" by using the clone command with a repository’s URL:

$ git clone https://github.com/test

### Coding: 

You enter the command **"code ."** so a VS code will open and modify the code as we wish. 

### Adding the files (Staging): 

Then I add the file that I have modified using the command **"git add ."** to add all the file I have modified. 

### Commiting file:

Next step is to commit the changes and inform what you did within the commit message as shown below:

$ git commit -m “made change x,y,z”

### Pushing Changes:

Then to push the changes to a remote repository as the following command:

$ git push origin master
