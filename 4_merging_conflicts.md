## Merging on GitHub (with Pull Requeest) & Dealing with Merge Conflicts ##

$ git checkout my_feature2

(commit some changes)

$ git push origin my_feature2

$ git checkout master

$ git difftool -y

(commit some conflicting changes)

$ git push origin master

(look on github)

(create PR on github)

(notice the conflict!)

Lets use a GUI to resolve our merge conflict - I use DiffMerge!

$ cat ~/.gitconfig

So, lets resolve by fixing *our branch*

$ git checkout my_feature2

$ git merge master

(conflicts...)

$ git mergetool

(resolve them)

$ git status

(lets create a merge commit)

$ git commit

$ git push origin my_feature2

(can add code review comments)
(can push more commits)

(show option to protect the master branch, enforce a code review approval, build checks) 

(refresh the PR, the conflict is resolved, now merge)

(delete branch in the gui)

git checkout master

git pull origin master

git remote prune origin