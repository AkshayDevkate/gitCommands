# gitCommands



To commit local code to remote repository 
 goto terminal/ command prompt > Navigate to project folder 
 
 git add .
 
 git commit -m "Write something"
 
 git push 
 "Error like
 ![rejected] master -> master (fetch first)
 error: failed to push some refs to git@"
 
 # Some times some one would have committed to the repository before you if you would like to overthrow the commits use following command 
 
 git push origin maste --force 
 
 Else 
 
 Stash your changes locally using command 
 
 git stash 
 
 than pull the changes that have been made to the repository by someone else using 
 
 git pull 
 
 now add your stashed changes to the repository on the top of changes made by someone else 
 
 git stash pop 
 
 
 ## Creating a branch 
 
 First you have to create a branch locally 
 git checkout -b <your_branch_name>
 
 After you create a branch locally, you can work locally in your branch. When you are ready to upload the code to new branch remote. The following command push the branch to remote repository origin and track it.
 
 git push -u origin <your_branch_name>
 
 Your team mates can look your branch using 
 
 git fetch
 or
 git checkout origin/<your_branch_name>
 
 
 Teammates can push to your branch by doing commits and then push explicitly
 
 ... work ...
git commit
... work ...
git commit
git push origin HEAD:refs/heads/your_branch

Or tracking the branch to avoid the arguments to git push

git checkout --track -b your_branch origin/your_branch
... work ...
git commit
... work ...
git commit
git push
 
