### PROJECT GIT WORKFLOW

- I created the project repo on GitHub
- After the project was created, I copied the project http url
- On my vscode terminal, I used "**git init**" to initialize the working directory on my local machine to track changes to my files.
- I used "**git remote add origin url**" to link my local directory to the github repo
- Then I used "**git checkout -b home-page**" to create feature branch for the home page
- After completing the home page for the mobile screen, I used "**git add .**" to stage my changes for the mobile screen.
- Then I used "**git commit -m 'added mobile responsiveness'**" to commit by staged files.
- I used "**git push -u origin home-page**" to push my local changes to GitHub.
- I created another branch "**git checkout -b location-page**" to create feature branch for the location page
- After, location page is done, I repeated line 8, 9 and 10 to push my changes to GitHub.
- Unfortunately, I realized at a point that, eventhough I have created a branch for the Home Page, I continued working on the master branch. For me to get the changes in master branch unto the Home Page, I checkedout into the Home Page with "**git checkout home-page**" and used "**git rebase master**" to merge the changes in master to home-page, and still get a cleaner commit history for the Home Page branch.
- I continued working in the Home Page branch and the Location Page branch respectively.
- After, I was done with the Home Page and the Location Page, I checked out into master and merged the respective branch changes into master using the command "**git merge home-page**" and "**git merge location-page**" respectively.
  -I had to rename the branches to suit AMALITECH branch naming convention using "**git branch -m feature/home-page**" and "**git branch -m feature/location-page**", after I checked into the respective branches.
  -Finally, I pushed the master branch to GitHub using "**git push -u origin master**".
