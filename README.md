# Cloud9-RoR1
RoR app using AWS Cloud9
Steps (from here: https://www.railstutorial.org/book/beginning#sec-prerequisites):
https://console.aws.amazon.com/
type “Cloud9” in the search box and choose it
click “Create environment”
section "Environment name and description"
Name = "rails-tutorial" and confirm till info about creating
Wait ~5 min, in "Project settings", "Ace", 'Soft tabs' = 2
Bottom window "bash...":
printf "install: --no-rdoc --no-ri\nupdate:  --no-rdoc --no-ri\n" >> ~/.gemrc
gem install rails -v 5.1.6
**************
Making a environment directory for Rails projects (!!!UNNECESSARY in the cloud).
$ cd               # Change to the home directory.
$ mkdir environment# Make a environment directory.
$ cd environment/  # Change into the environment directory
*************
cd ~/environment # Change into the environment directory
rails _5.1.6_ new hello_app #create new RoR app
*************
GIT: #go to your project directory
git status #info about project files

git init #start using git for project
git add . #add all project files to check status
git commit -m "your comment" #prepare files for commit
git rm file.fff #remove file from checking list (not physical deleting)

#add remote repo. with alias 'hw' and url = 'git://....'
git remote add hw git@github.com:<MyGitAccountName>/hw.git #ssh method
git remote add hw git://github.com/<MyGitAccountName>/hw.git #https method
#get info about remotes: git remote -v
#get all new files and put in your project: git pull
#delete remote rep: git remote rm ww # alias = 'ww'

        ++++++MOST IMPORTANT++++++
#create new remote repo:
    curl -u '<MyGitAccountName>' https://api.github.com/user/repos -d '{"name":"NewRep"}'
#push an existing repository to remote:
1.    git remote add origin https://github.com/<MyGitAccountName>/NewRep.git
#if you have any error do this: git remote rm origin #then repeat step 1.
2.    git push origin master
#after your work with files do this: 
    git commit -m "your comment" -a #commit all changes
#or you can add only part of files to commit: git add [file_name]
    git push origin master #push to remote
*************
start Rails server:
cd ~/environment/hello_app/ #change env to current app
rails s #start server
