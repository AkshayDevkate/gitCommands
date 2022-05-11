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
 
 
