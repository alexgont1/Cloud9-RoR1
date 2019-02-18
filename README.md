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