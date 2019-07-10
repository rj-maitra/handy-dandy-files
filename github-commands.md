# Pushing code from your computer to GitHub

I've parsed the internet and put together these simple instructions to get you up and running.

### Setting up Git 
* http://git-scm.com/book/en/v2/Getting-Started-Installing-Git
  * Follow the commands for your computer
* Setting up your username and email address:
  * `git config --global user.name "<your first and last name>"` (include the quotes, and no angle brackets!)
  * `git config --global user.email <your GitHub email address>` (no quotes or angle brackets)
  * Verify with `git config --global --list`
  
### When you `git init` in your terminal, you are creating a repository on **YOUR** computer.  These are the steps you would follow after making a project and `cd`'ing into the **project** folder.
* `git add .` will add all the files in the current folder/directory (i.e. your project folder) to staging
* `git commit -m "text"` will tag the "text" to the files as a comment
* If you modify something, type in `git status` to find what has been modified and not staged.  The below commands are for modified files.
  * Type in `git diff` to find differences in the actual files you modified
  * `git add .` will add all the changed files to the staging area
  * `git commit -m "text"` again to tag the latest changed files with a comment
  * `git log` to see the "paper trail"

### Go to GitHub.com and set up a new repository ON GitHub.
* After making the repo, you are presented with two sets of commands:
  * Create a new repository
  * Push to an existing repository
* If you have already made something on your computer, it is an **EXISTING** repository, and you will:
  * `git remote add origin <url>` (link from the new repo page on GitHub, no angle brackets)
  * `git push -u origin master` (pushes the master branch and makes it the origin)
