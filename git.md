# Steps to starting the git

Step-1->    ENABLE GIT IN PROJECT BY             ( git init) 
            It enables the git to start tracking this folder, this makes a new .git folder it is hidden folder. It contains all the information of the versions or commits done up till now.

Step-2->    (git status)It tells about files which are tracked and are not tracked by the git.
             

             ``` Text
             There are 3 stages of any file 
             1st- >  Working directory  (These places in which the git does not track about the changes done the file, or it does not saves the current changes .)

             2nd- > Staging area    (git add <FileName>) (It starts tracking that perticular file , if something is in the staging area it will probably be a part of the next version / commit)

             3rd- > Repository (git commit) it will commit the files which are currently present at the staging area.
             
             ```

Step-3->  Use command { git commit -m "add massage" }to commit and add massage to the file which will have to be commited.


``` text
->> All the files which are created , or modified but are not staged (i.e. git add <filename>) will be present in Working directory.

->> All the files which are beeing tracked and are the part of next version and are not the part of working directory all such files are present in Staged area

-->> All the staged file after being commit wil be than shifted to Repository (and this repository will be a local repository.)

-->> From the local repository (distributed) we can shift it to (central) repository which can be online like github, gitlab, BitBucket.

-->> What is diffrence between git and github?

-->> Create a remote github repo attach that repo with the local repo

-->> After doing commit all the changes done wiil be saved into the local repository not in the online repo. to make that commit to available in online repository of github we have to use command "git push origin main."
```
Stash :->>  This allow us to save changes of "working directory or staged area" without commiting them. These changes are saved independently from the other files which are commited.

(git stash)  -->> This Command will stash the "changes of staging area and tracked files of working directory and not of untracked files of working directory".

(git stash list)    -->> THis Command will show the list of changes which are stashed.

(git stash push -m "Write your message") :->> Using this command we can stash the changes along with a proper message.

->> The changes which are added into the stash are added in stack formate that LIFO.

(git stash clear) :-> Using this command we can clear the all the list of stash changed

(git stash --include-untrack) : This command is used to add changes of untracked files in stash.

(git stash apply) :- THis command is used to apply the last change you have stashed, but it does not remove the last stash from stash list.

(git stash pop) :- THis command is used to apply the last change you have stashed ,and also it removes the last stash from stash list.

(git stash drop @stash{x}) :- This remove the specific stach (i.e. stash number{x}) from the stash list.

(git stash apply stash{x}) :- This command apply the specific stash number {x} from the stash list.

# This line is writeen in the main branch not on the master Branch.
1. Now I will pull this line into the master branch.
   
