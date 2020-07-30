# 2020/07/30: Git Collaboration

Git collaboration notes

## Branches

- `git clone <url>`: downloads the repository from the web to your local computer
    - make sure you don't nest this command into another repository
    - just like `git init`, only do this once per repo

- `git branch <branch_name>`: create a new branch where HEAD is
    - `git branch -a`: list all the branches your local machine knows of
- `git switch <branch_name>`: move to branch
    - `git checkout <branch_name>`: the pre-august 2019 way

- `git switch -c <branch_name>`: create and move to branch in 1 step
    - `git checkout -b <branch_name>

## Pull Requests (Online Merge)

- `git log --oneline --graph --decorate --all`: shows you your git history tree
    - you can look up how to set this as an git alias

- `git fetch --prune`: clean your git history, and remove references from remote that no longer exist

- `git branch -d <branch_name>`: removes branch from your local computer

- Pull request: when you push a branch to the remote, and merge the branch in the online interface

# Some additional notes and links

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
