# GIT-DOCS

  # git is a source code management tool 

  # git and gitHub both are different, gitHub(cloud) is central repository by using git we pass code to the gitHub repository

  # git is software that we installed in our machine

  # to install git , here's url to download git https://github.com/git-for-windows/git/releases/download/v2.55.0.windows.5/Git-2.55.0.5-64-bit.exe

  # to create gitHub account,  here's the url to create gitHub account https://github.com/signup

  # after installing git we need to add git install command once to initialize the git in the specific folder

  # here''s the command to initialize git in specific folder
       # git init

  # when we initialize git using git init command by default branch is main , to check the branches we are using
       # git branch --list (it will show the all the branches created by you)

  # if you want to create branch , need to run this command
       # git branch branchName
 
  # after creating the branch we need to checkout to the branch to add changes from that branch, here's the command to checkout
       # git checkout branchName

   # we can able to create and checkout branch in single command, here's the command
       # git checkout -b branchName

  # we need to configure username and email in the git software 
  
  # here's the commands to add username and email
       # git config --global user.name "username"
       # git config --global user.email "useremail"

  # to check the username and email use this command
       # git config --list

  # in git we have three phases to transfer data from git to gitHub(cloud)

  # here's the phases
       # workSpace 
       # staging/index
       # local repository

  # need to pass changes from one phase another phase only way to pass data using git to gitHub

  # if we want to check the status of the changes we are using 
       # git status 

  # if we want to pass changes from first phase to second phase we are using 
       # if the changed file is in first phase it is appear in red color when we check the status
       # git add fileName (it means a specific file) / git add . (it means all changed files)

  # if we pass changes from second phase to third phase we are using
       # if the changed file in second phase it's appear in green color when we check the status
       # git commit -m "commit message to track the changes"

  # we can able to hide changes in between second phase and third phase , here's the commands
       # git stash (to hide the changes)
       # git stash apply/pop (to show the changes)

  # if we pass changes from third phase to git hub we are using
       # if the changed files in third phase it is shows like nothing to commit , working tree clean , when we check the git status
       # git push --set-upstream origin branchName / git push 
       # before pushing the code to gitHub need to take latest pull from gitHub / parent branch / feature branch to avoid conflicts, here's the command
       # git pull (it will automatically take the commits from the repository without doing merge or rebase)
       # git fetch (it will fetch the commit history from repository but we need to merge / rebase)


  # how merge conflicts will happen and how to avoid it
       # if you are working in one file and other persons also working on the same file , in this case if you push your code on first in the parent branch there's no issues found for you but after someone try to push the code without taking latest pull from the parent branch at that time another person face merge conflicts it means , someone added these changes and you are added these changes (current, incoming changes) which one is the correct and which one needs to avoid , this is the way we can resolve merge conflicts, to avoid merge conflicts whenever pushing the changes in parent branch better to take pull from the parent branch and then resolve issues in local and pushing the code to the parent is avoid merge conflicts

  # we can able to merge one branch into another  , by using this command
       # git merge branchName (first we need to checkout to the base branch and run this command with the branch need to merge)
       # it will not modified the history but little messy in the structure (history is not in linear format)
       # it will helps to track the history better to use in merges feature branch to main branch
       # git rebase branchName is also similar to merge the branches but it rewrites the history
       # git squash is used to combine multiple commits into single commit





