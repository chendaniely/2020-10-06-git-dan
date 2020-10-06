# 2020/10/06: Git Basics Notes

Local and Remote notes for Git

Change from branch


Additional resources:

- git + rstudio: https://happygitwithr.com/
- dan's reference guide for git (but uses branches): https://chendaniely.github.io/training_ds_r/help-faq.html
- swc git lesson: https://swcarpentry.github.io/git-novice/
- if you want to know more about branches and forks: https://www.youtube.com/watch?v=uvWhSYBkZJ0
- Setting up ssh links: https://bi-sdal.github.io/training/ssh-keys.html

- Software Carpentry notes on basic git: https://swcarpentry.github.io/git-novice/
    - The setting up git has the commands to setup your name/email/editor: https://swcarpentry.github.io/git-novice/02-setup/index.html

- Git workflow notes and commands (to paste on your wall)
    - https://chendaniely.github.io/training_ds_r/help-faq.html

- Atlassian page on git workflows: https://www.atlassian.com/git/tutorials/comparing-workflows
    - The one we covered today was mainly the "Feature Branch Workflow": https://www.atlassian.com/git/tutorials/comparing-workflows/feature-branch-workflow

- The atlassian page has more infor about "git flow", but this is also another top Google hit that I liked:
  - https://nvie.com/posts/a-successful-git-branching-model/

- Getting your (bash) terminal to show current path and other things:
    - Use this to create your PS1 variable: http://bashrcgenerator.com/

- Show git branch in terminal:
    - In addition you can write a function and put that in your PS1 to also show git branch
    - https://gist.github.com/joseluisq/1e96c54fa4e1e5647940


## Local

- `git init`: create git respotiroy in current folder
    - you only do this one per repository
    - do not nest git repositories
- `git status`: tells you what is going on in your repository
- `git add <files>`: puts <files> into the staging area (index)
- `git commit`: commit message for files in staging area
    - `git commit -m "MESSAGE"`: oneline commit message wihtout opening up the text editor
- `git log`: show you your log history
    - `git log --oneline`: one line version of your history

- `git diff`: will show you the differences
    - `git diff --staged`: show you differences in the staging area
    - `git diff HEAD~2`: diff 2 places back from HEAD
    - `git diff <HASH>`: diff 2 locations

- `git checkout <HASH> <FILE>`: revert file
- `git checkout <HASH>`: go to location
- `git checkout master`: go back to master

## Remotes

- `git remote add origin <URL>`: adds the url with the name "origin"

- `git push origin master`: sends master branch on local computer to remote
- `git pull origin master`: updates local with remote (master)

- GitHub allows you to edit files online using the pencil (plain text files)
