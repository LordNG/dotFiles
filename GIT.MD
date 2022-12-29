# GIT instuctions:

### Create repository:
##### on server
create an empty dir:
``mkdir project.git``

go to created dir:
``cd project.git``

create bare .git dir:
git init --bare``

##### on other computer
create an empty dir:
``mkdir project.git``

go to created dir:
``cd project.git``

create .git dir:
``git init``

add files to stage:
``git add .``

add commit message:
``git commit -m 'Initial commit'``

set remote:
``git remote add origin git@server:/path/to/project.git``

push changes:
``git push origin master``
  or
``git push --set-upstream origin master``




### Git branching:
create a new branch:
``git branch test``

switching branch:
(make sure to commit changes before switching branch by checking git status)
``git checkout testing``



### Squashing multiple commits into 1 commit:
#### from other branch
Check out the target branch (eg: master):
``git checkout master``

merge the working branch (eg: test):
``git merge --squash test``

commit new message:
``git commit

push upstream:
``git push``



