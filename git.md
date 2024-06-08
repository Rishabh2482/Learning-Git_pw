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
```