This project is for the code for FRC Team 525's robot for the 2018 FIRST Power Up Season.

A quick overview of how to use git:

Git is a utility that allows for multiple programmers to collaborate on a project from multiple computers from anywhere in the world. Our repository on GitLab (https://gitlab.com/crm11396/2018_Swartdogs_Power_Up_Robot_Code)
has a collection of lists of issues that can be tackled. These lists can be found by navigating to "Issues > Boards" when viewing our repository online. Any tasks that haven't been started will be in the list labelled "Backlog". 
Tasks that are currently being worked on will be in the list labelled "In Progress". Tasks that are completed and are ready to be merged (explained below) will be in the list labelled "Ready To Merge". Tasks that are completely 
finished are in the list labelled "Closed".

Git uses a method of organization involving branches. From a particular point in the development process, users can create "branches", which are essentially personal copies of the project that users can modify. To create a
branch, run the command "git checkout -b <new branch name>". In order to switch to a different, existing branch, run the command "git checkout <existing branch name>". When the modifications are complete, the user can merge 
their branch into the main (or "master") branch where all of the completed code is. To merge a branch into the master branch, the user must submit a merge request from the online repository. Merge requests give the entire team 
a chance to see what changes to the code have been made, and each user can give feedback/suggestions on the code. For our team, changes must be approved by a mentor before they can be merged into the master branch.

Common convention for using git involves creating a new branch for each task listed in the "Backlog" list, writing the code to complete the task, submitting a merge request, and ultimately merging the new branch into the master
branch once the changes have been approved. When all is said and done, the master branch will contain a final version of the code that will be deployed to the robot.

When writing the code for a particular task, users can essentially save their progress at various points. These save points are called "commits" and programmers can revert to any individual commit if changes have been made that
need to be undone. When the programmer wants to merge a branch into another branch, they can choose to either merge every commit (every save point) or only the final commit (only the last save point). More commits means more
places to revert to, but is also more information to sift through and can make navigation more difficult.

To create a commit, programmers will need to enter a series of commands into the git bash (a git-enabled command line window). The programmer first needs to tell git what files should be saved in the commit. To do this, enter the
command "git add <files to commit>". Typically, you'll want to commit every file in the workspace, and you can do this with the command "git add .". Once git knows all of the files that should be committed, you can create the
commit with the command 'git commit -m "commit message"'. The commit message is generally only a couple of words, maybe a sentence or two at the most. The message will provide a brief description of what the commit contains.
Examples include "Added comments to drive.cpp" and "Tuned PID control for drive rotation".

Once the commit is created, the commit is only visible on the computer where it was made. In order for the rest of the team to see the commit (or to be able to access the commits from a different computer), the commit must be
pushed to the online repository. To do this, run the command "git push origin <branch name>". The commit will now be pushed to our online repository. In order to download the commit to a different computer, run the command
"git pull origin <branch name>".

If you have questions about how to use git, there's some pretty good documentation online, but you can also ask me any questions by emailing me at crm11396@gmail.com.