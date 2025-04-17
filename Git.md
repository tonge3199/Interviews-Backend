## SSH vs HTTPS for Git

All as authentication method.

The two protocols differ in terms of complexity and level of security.

SSH (Secure Shell) is a public-key cryptography protocol that ensures no one can intercept or change the data during the transfer.

it offers greater data integrity (数据完整性) and security.

## Git Commands

Git **merge**, rebase区别？

in branch main, git merge other_branch (into main)

**Fast Forward Merge** 

Merge ​合并分支​​：创建新的合并提交，保留两个分支的完整历史

Rebase ​变基​​：将当前分支的提交"嫁接"到目标分支的最新提交之后，重写提交历史

远程分支A->B->C,本地分支A->D->E,分别merge和rebase之后是什么状态?

其他Git命令:

git status

git add <>

git commit -m ""

git log --oneline/--decorate=no

+ git log --oneline --graph --all

git config --add/--unset(-all) k.v/ --unset-section

+ git config --global init.defaultbranch main

git branch -m oldname newname / -d delete_branch

git switch -c (create) new_branch 

git checkout

git restore 

git reset --soft/hard <HASH>

git remove file

**git rebase** : eg. bring changes from main into feature_branch, git rebase avoids a merge commit
by replaying the cmommits from feature_branch on top of main

git remote add <name> <uri>

git fetch

git pull

git push

git fork work flow:

1.Fork the main repo

2.Clone down forked repo to own environment

3.Make the changes to the main branch in the forked repo

4.Push changes to the main branch in the forked repo

5.Open a PR with the changes from the fork onto the original repo

(second remote upstream : point to the origin)

**git reflog**

git cat-file -p HASH :查看这个提交的内容。该命令会显示提交信息和tree哈希

git ls-tree