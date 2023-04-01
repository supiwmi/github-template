[![Codespaces Prebuilds](https://github.com/supiwmi/github-template/actions/workflows/codespaces/create_codespaces_prebuilds/badge.svg)](https://github.com/supiwmi/github-template/actions/workflows/codespaces/create_codespaces_prebuilds)
[![CI](https://github.com/supiwmi/github-template/actions/workflows/cicd.yml/badge.svg)](https://github.com/supiwmi/github-template/actions/workflows/cicd.yml)

# github-template
codespaces template for devops

## Git - Tips and Tricks
```
* git status
1. check status of our repo
2. what's been added
3. how many files changed

* git add A
adding all files/changes

* git add .
adding new or existing files to stagging, without thosed deleted

* git diff
display changes against last commit

* git pull
pull changes from the remote repo

* git checkout -b
create a new branch or new "version" of the code

* git checkout
switch to existing branch

* git branch
display the current branch

* git merge <branch>
bring changes in from another branch

```
Example:

In this example we will create a development branch and adding a new code, after then we commit the change and merge it to the main branch
1. git checkout -b dev-branch

Let's make some changes so the dev-branch (new version) branch is newer than the main(stable version)
1. git add .
2. git commit -m "adding new functions in development branch"
3. git push origin dev-branch

Create a Pull Request to merge dev-branch into --> main branch (so you need to switch to the main and issue git merge command
1. git checkout main
2. git merge dev-branch 

## Tips
1. You may create the 3rd brach called "feature-branch" and then try to merge new code to dev-branch instead of main.
2. You can create a Pull Request from Git Repo(GitHub, Bitbucket, etc.) or use the git cli as show in the example above.

