# A Beginners Guide to Git (Because the beginner is the writter)

## A. Download 

### https://git-scm.com/downloads

## B. How to set up git 

### *Global Setup*

#### `git config --global user.name "YourNameHere"`
#### `git config --global user.email "youremail@here.com"`

### *Repository Setup*

#### `git config user.name "YourNameHere"`
#### `git config user.email "youremail@here.com"`

## C. Getting Started

### Download Git Repository

#### `git clone https://github.com/michaelcw02/Sudoku.git`

## D. Basics

### *Adding untracked files*
This is mainly for new files that are added into the local repository
#### `git add *` 
##### if you want to add everything in the folder
#### `git add specific.ext` 
##### if you want to add the specific file

### *Committing*
This is like a "checkpoint" of what you have done. It is like this because it gives you the possibility to "regret" and go back to certain "checkpoint"
#### `git commit -a -m "A comment of what you have done"`

### *Pushing*
After doing finishing your work you can do a push, that it is like a "save", that can be done by
#### `git push`
OR
#### `git push -u origin BranchName`

### *Pulling*
This is done in order to get the latest updates on the current branch you might be working on.
#### `git pull`
    It is recommended to do this command everytime you are going to start working on something

### *Fetching*
    TO-DO

## E. Branching
A branch is like a "feature" that you want to do, and you do not want to affect the state of the original 

#### `git branch`
This is to know all the existing branches locally
*Note that there could be branches that are on Github, but not on your repo*

#### `git checkout -b (NewBranchName)`
This is to create a new branch and "go" to that branch

#### `git checkout (ExistingBranchName)`
This is to change the branch you are currently working on

#### `git branch -d (ExistingBranchName)`
This is to delete the current branch locally

#### `git merge (NameofTheBranchYouWantToMergeWith)`
This command will merge your changes with the another branch. If you commit and push normally, you will change the current branch you are in

#### `git rebase BranchAName BranchBName`
Get the changes from branch B, and then updates it with branch A changes

## F. Conflict managing
Personally I like to use Visual Studio Code to manage the conflicts
### https://code.visualstudio.com/download

In order to manage this, you should have the whole repository open in Visual Studio Code
