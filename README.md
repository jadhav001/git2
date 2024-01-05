PS D:\full stack> cd git
PS D:\full stack\git> git clone https://github.com/jadhav001/repo-name1.git
Cloning into 'repo-name1'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (6/6), done.
PS D:\full stack\git> ls


    Directory: D:\full stack\git


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        04-01-2024     20:47                repo-name1


PS D:\full stack\git> ls -a
Get-ChildItem : Parameter cannot be processed because the parameter name 'a' is 
ambiguous. Possible matches include: -Attributes -Directory -File -Hidden -ReadOnly 
-System.
At line:1 char:4
+ ls -a
+    ~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem], ParameterBindin 
   gException
    + FullyQualifiedErrorId : AmbiguousParameter,Microsoft.PowerShell.Commands.GetC 
   hildItemCommand
 
PS D:\full stack\git> ls -l
Get-ChildItem : Missing an argument for parameter 'LiteralPath'. Specify a 
parameter of type 'System.String[]' and try again.
At line:1 char:4
+ ls -l
+    ~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem], ParameterBindin 
   gException
    + FullyQualifiedErrorId : MissingArgument,Microsoft.PowerShell.Commands.GetChil 
   dItemCommand
 
PS D:\full stack\git> ls -la
Get-ChildItem : A parameter cannot be found that matches parameter name 'la'.
At line:1 char:4
+ ls -la
+    ~~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem], ParameterBindin  
   gException
    + FullyQualifiedErrorId : NamedParameterNotFound,Microsoft.PowerShell.Commands.  
   GetChildItemCommand

PS D:\full stack\git> git status
fatal: not a git repository (or any of the parent directories): .git
PS D:\full stack\git> git status
fatal: not a git repository (or any of the parent directories): .git
PS D:\full stack\git> ls


    Directory: D:\full stack\git


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        04-01-2024     20:54                repo-name1


PS D:\full stack\git> cd repo-name1
PS D:\full stack\git\repo-name1> ls -a
Get-ChildItem : Parameter cannot be processed because the parameter name 'a' is      
ambiguous. Possible matches include: -Attributes -Directory -File -Hidden -ReadOnly  
-System.
At line:1 char:4
+ ls -a
+    ~~
    + CategoryInfo          : InvalidArgument: (:) [Get-ChildItem], ParameterBindin  
   gException
    + FullyQualifiedErrorId : AmbiguousParameter,Microsoft.PowerShell.Commands.GetC  
   hildItemCommand

PS D:\full stack\git\repo-name1> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        css.css
        html.html
        js.js

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\full stack\git\repo-name1> git add html.html
PS D:\full stack\git\repo-name1> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   html.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        css.css
        js.js

PS D:\full stack\git\repo-name1> git add css.css  
PS D:\full stack\git\repo-name1> git add js.js  
PS D:\full stack\git\repo-name1> git status     
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   css.css
        new file:   html.html
        new file:   js.js

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

PS D:\full stack\git\repo-name1> git add .    
PS D:\full stack\git\repo-name1> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md
        new file:   css.css
        new file:   html.html
        new file:   js.js

PS D:\full stack\git\repo-name1> git commit -m "new files added"
[main 9eb0dbb] new files added
 4 files changed, 13 insertions(+)
 create mode 100644 css.css
 create mode 100644 html.html
 create mode 100644 js.js
PS D:\full stack\git\repo-name1> git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS D:\full stack\git\repo-name1> git push origin main
info: please complete authentication in your browser...
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 538 bytes | 538.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/jadhav001/repo-name1.git
   0a8e0ed..9eb0dbb  main -> main
PS D:\full stack\git\repo-name1> cd ..
PS D:\full stack\git> cd ..
PS D:\full stack> mkdir git2


    Directory: D:\full stack


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        04-01-2024     21:54                git2


PS D:\full stack> cd git2
PS D:\full stack\git2> ls


    Directory: D:\full stack\git2


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        04-01-2024     21:55              0 demo.css
-a----        04-01-2024     21:54              0 demo.html
-a----        04-01-2024     21:55              0 demo.js


PS D:\full stack\git2> git status
fatal: not a git repository (or any of the parent directories): .git
PS D:\full stack\git2> git init
Initialized empty Git repository in D:/full stack/git2/.git/
PS D:\full stack\git2> git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        demo.css
        demo.html
        demo.js

nothing added to commit but untracked files present (use "git add" to track)
PS D:\full stack\git2> git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add
PS D:\full stack\git2> git add .
PS D:\full stack\git2> git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   demo.css
        new file:   demo.html
        new file:   demo.js

PS D:\full stack\git2> git commit -m "uplode from local system"
[main (root-commit) 443e6bc] uplode from local system
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 demo.css
 create mode 100644 demo.html
 create mode 100644 demo.js
PS D:\full stack\git2> git status
On branch main
nothing to commit, working tree clean
PS D:\full stack\git2> git push origin main
fatal: 'origin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
PS D:\full stack\git2> touch README.md     
PS D:\full stack\git2> git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
PS D:\full stack\git2> git add .
PS D:\full stack\git2> git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   README.md

PS D:\full stack\git2> git commit -m "redme file uplode from local system"
[main 72c882d] redme file uplode from local system
 1 file changed, 2 insertions(+)
 create mode 100644 README.md
PS D:\full stack\git2> git status
On branch main
nothing to commit, working tree clean
PS D:\full stack\git2> git remote add origin https://github.com/jadhav001/git2.git
PS D:\full stack\git2> git remote -v
origin  https://github.com/jadhav001/git2.git (fetch)
origin  https://github.com/jadhav001/git2.git (push)
PS D:\full stack\git2> git branch
* main
PS D:\full stack\git2> git push origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 501 bytes | 62.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/jadhav001/git2.git
 * [new branch]      main -> main
PS D:\full stack\git2> git branch -M master
PS D:\full stack\git2> git branch
* master
PS D:\full stack\git2> git branch -M main  
PS D:\full stack\git2> git branch        
* main
PS D:\full stack\git2> git push -u  origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.
PS D:\full stack\git2> git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\full stack\git2> git commit -m "redme file uplode from local system add"    
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\full stack\git2> git add .           
PS D:\full stack\git2> git commit -m "redme file uplode from local system add"
[main 50feef4] redme file uplode from local system add
 1 file changed, 3 insertions(+), 1 deletion(-)
PS D:\full stack\git2> git push                
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 353 bytes | 353.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/jadhav001/git2.git
   72c882d..50feef4  main -> main
PS D:\full stack\git2> git chechout -b feture
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout
PS D:\full stack\git2> git checkout -b second branch
fatal: 'branch' is not a commit and a branch 'second' cannot be created from it
PS D:\full stack\git2> git checkout -b secondh      
Switched to a new branch 'secondh'
PS D:\full stack\git2> git branch                   
  main
* secondh
PS D:\full stack\git2> git checkout -d
HEAD is now at 50feef4 redme file uplode from local system add
PS D:\full stack\git2> git checkout   
PS D:\full stack\git2> git branch     
* (HEAD detached at 50feef4)
  main
  secondh
PS D:\full stack\git2> git branch main
fatal: a branch named 'main' already exists
PS D:\full stack\git2> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\full stack\git2> git checkout -d secondh
HEAD is now at 50feef4 redme file uplode from local system add
PS D:\full stack\git2> git checkout           
PS D:\full stack\git2> git checkout main      
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\full stack\git2> git branch             
* main
  secondh
PS D:\full stack\git2> git branch -d secondh  
Deleted branch secondh (was 50feef4).
PS D:\full stack\git2> git branch
* main
PS D:\full stack\git2> git checkout -b newbch    
Switched to a new branch 'newbch'
PS D:\full stack\git2> git branch
  main
* newbch
PS D:\full stack\git2> git status            
On branch newbch
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        new .js

nothing added to commit but untracked files present (use "git add" to track)
PS D:\full stack\git2> git add . 
PS D:\full stack\git2> git commit "new"
error: pathspec 'new' did not match any file(s) known to git
PS D:\full stack\git2> git commit -m "new"
[newbch fcfb22f] new
 1 file changed, 1 insertion(+)
 create mode 100644 new .js
PS D:\full stack\git2> git status         
On branch newbch
nothing to commit, working tree clean
PS D:\full stack\git2> git push
fatal: The current branch newbch has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin newbch

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS D:\full stack\git2> git push origin main
Everything up-to-date
PS D:\full stack\git2>     git push -u origin newbch            
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 260 bytes | 260.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'newbch' on GitHub by visiting:
remote:      https://github.com/jadhav001/git2/pull/new/newbch
remote:
To https://github.com/jadhav001/git2.git
 * [new branch]      newbch -> newbch
branch 'newbch' set up to track 'origin/newbch'.
PS D:\full stack\git2> git push
Everything up-to-date
PS D:\full stack\git2> git add .
PS D:\full stack\git2> git branch
  main
* newbch
PS D:\full stack\git2> git add . 
PS D:\full stack\git2> git commit -m "commit"
[newbch 6ec68cc] commit
 1 file changed, 1 insertion(+), 1 deletion(-)
PS D:\full stack\git2> git branch
  main
* newbch
PS D:\full stack\git2> git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 252 bytes | 50.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/jadhav001/git2.git
   fcfb22f..6ec68cc  newbch -> newbch
PS D:\full stack\git2> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS D:\full stack\git2> git branch 
* main
  newbch
PS D:\full stack\git2> git diff newbch
diff --git a/new .js b/new .js
deleted file mode 100644
index 10b07d8..0000000
--- a/new .js
+++ /dev/null
@@ -1 +0,0 @@
-//new SS
\ No newline at end of file
PS D:\full stack\git2> git branch     
* main
  newbch
PS D:\full stack\git2> git checkout newbch
Switched to branch 'newbch'
Your branch is up to date with 'origin/newbch'.
PS D:\full stack\git2> git pull origin main
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (1/1), 622 bytes | 1024 bytes/s, done.
From https://github.com/jadhav001/git2
 * branch            main       -> FETCH_HEAD
   50feef4..776c08b  main       -> origin/main
Updating 6ec68cc..776c08b
Fast-forward
PS D:\full stack\git2> git checkout newbch 
Already on 'newbch'
Your branch is ahead of 'origin/newbch' by 1 commit.
  (use "git push" to publish your local commits)
PS D:\full stack\git2> git checkout main  
Switched to branch 'main'
Your branch is behind 'origin/main' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)
PS D:\full stack\git2> git pull origin main
From https://github.com/jadhav001/git2
 * branch            main       -> FETCH_HEAD
Updating 50feef4..776c08b
Fast-forward
 new .js | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 new .js
PS D:\full stack\git2> git branch
* main
  newbch
PS D:\full stack\git2> git add . 
PS D:\full stack\git2> git commit -m "coomit" 
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
PS D:\full stack\git2> git add .
PS D:\full stack\git2> git commit -m "coomit" 
[main 11b2ce4] coomit
 1 file changed, 1 insertion(+), 1 deletion(-)
PS D:\full stack\git2> git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS D:\full stack\git2> git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS D:\full stack\git2> git checkout newbch 
Switched to branch 'newbch'
Your branch is ahead of 'origin/newbch' by 1 commit.
  (use "git push" to publish your local commits)
PS D:\full stack\git2> git add .
PS D:\full stack\git2> git commit -m "coomit" 
[newbch e786e0d] coomit
 1 file changed, 1 insertion(+), 1 deletion(-)
PS D:\full stack\git2> git checkout main  
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
PS D:\full stack\git2> git add .
PS D:\full stack\git2> git commit -m "coomit" 
[main 145ad75] coomit
 1 file changed, 1 insertion(+), 1 deletion(-)
PS D:\full stack\git2> git branch
* main
  newbch
PS D:\full stack\git2> git checkout newbc
error: pathspec 'newbc' did not match any file(s) known to git
PS D:\full stack\git2> git checkout newbh
error: pathspec 'newbh' did not match any file(s) known to git
PS D:\full stack\git2> git checkout newbch
Switched to branch 'newbch'
Your branch is ahead of 'origin/newbch' by 2 commits.
  (use "git push" to publish your local commits)
PS D:\full stack\git2> git marge main     
git: 'marge' is not a git command. See 'git --help'.

The most similar command is
        merge
PS D:\full stack\git2> git merge main
Auto-merging new .js
CONFLICT (content): Merge conflict in new .js
Automatic merge failed; fix conflicts and then commit the result.      
PS D:\full stack\git2> git merge main
error: Merging is not possible because you have unmerged files.        
hint: Fix them up in the work tree, and then use 'git add/rm <file>'   
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.
PS D:\full stack\git2> git add .
PS D:\full stack\git2> git commit -m "coomit"
[newbch 50da1ec] coomit
PS D:\full stack\git2> git merge main
Already up to date.
PS D:\full stack\git2> git push
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 8 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (12/12), 917 bytes | 917.00 KiB/s, done.
Total 12 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 1 local object.   
To https://github.com/jadhav001/git2.git
   6ec68cc..50da1ec  newbch -> newbch
PS D:\full stack\git2> git add .
PS D:\full stack\git2> git status
On branch newbch
Your branch is up to date with 'origin/newbch'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   new .js

PS D:\full stack\git2> gir reset
gir : The term 'gir' is not recognized as the name of a cmdlet, 
function, script file, or operable program. Check the spelling of the  
name, or if a path was included, verify that the path is correct and   
try again.
At line:1 char:1
+ gir reset
+ ~~~
    + CategoryInfo          : ObjectNotFound: (gir:String) [], Comman  
   dNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException

PS D:\full stack\git2> git reset
Unstaged changes after reset:
M       new .js
PS D:\full stack\git2> git reset new js
fatal: ambiguous argument 'new': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
PS D:\full stack\git2> git reset new.js
fatal: ambiguous argument 'new.js': unknown revision or path not in the working tree.
Use '--' to separate paths from revisions, like this:
'git <command> [<revision>...] -- [<file>...]'
PS D:\full stack\git2> git status      
On branch newbch
Your branch is up to date with 'origin/newbch'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   new .js

no changes added to commit (use "git add" and/or "git commit -a")      
PS D:\full stack\git2> git add .       
PS D:\full stack\git2> git commit -m "rere"
[newbch ce822e9] rere
 1 file changed, 2 insertions(+), 1 deletion(-)
PS D:\full stack\git2> git status
On branch newbch
Your branch is ahead of 'origin/newbch' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS D:\full stack\git2> git reset HEAD
PS D:\full stack\git2> git status    
On branch newbch
Your branch is ahead of 'origin/newbch' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
PS D:\full stack\git2> git reset HEAD~1
Unstaged changes after reset:
M       new .js
PS D:\full stack\git2> git status      
On branch newbch
Your branch is up to date with 'origin/newbch'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   new .js

no changes added to commit (use "git add" and/or "git commit -a")      
PS D:\full stack\git2> git log
commit 50da1ec4044694c171b055a723ba3b1f15c8ab13 (HEAD -> newbch, origin/newbch)
Merge: e786e0d 145ad75
Author: sumitjadhav <sumitjadhav3630@gmail.com>
Date:   Fri Jan 5 00:45:54 2024 +0530

    coomit

commit 145ad755e2ad3052db0285da6c4b5fafa3d4b394 (main)
Author: sumitjadhav <sumitjadhav3630@gmail.com>
Date:   Fri Jan 5 00:40:09 2024 +0530

    coomit

commit e786e0d4d4ba9a576b4b5aede58269429294c74d
Author: sumitjadhav <sumitjadhav3630@gmail.com>
Date:   Fri Jan 5 00:39:29 2024 +0530

    coomit

commit 11b2ce4ff2c29435e43187b59332999bf26a2706
Author: sumitjadhav <sumitjadhav3630@gmail.com>
Date:   Fri Jan 5 00:36:42 2024 +0530

    coomit

commit 776c08bd56be070687d6917c4393b483ce0ac787 (origin/main)
Merge: 50feef4 6ec68cc
Author: jadhav001 <147920870+jadhav001@users.noreply.github.com>       
Date:   Fri Jan 5 00:24:35 2024 +0530
: