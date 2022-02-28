## How to Contribute in this Project (Git Work Flow)

### 1. **Fork the Repository**
  - Click the fork button to fork the repository. 
  - It will make a copy of repository under your account. 
  - Changes will not reflect in original one until pull request is merged by owner of the repository.
  
### 2. **Clone Forked Repository**
  - Click on code button.
  - Select https or ssh (if ssh key is already setuped).
  - Click on copy icon.
  - Then, type the following *git clone* command in terminal to clone into your machine locally.
  
```
git clone "git@github.com:<your-username>/SIH2022-DR716.git"
```
replace <your-username> with your github username or basically just paste copied link in terminal.

### 3. **Configure remote upstream to original Repo(link forked to original one - *__need to do it only once__*)** 
  - This command links to the original repo (just do it once).
  - Type the following *git remote* command on terminal
  
```
git remote add upstream git@github.com:Navdeepsingh4298/SIH2022-DR716.git
```
  - In this example, 'upstream' is the shortname we have supplied for the remote repository since in terms of Git, "upstream" refers to the repository that you cloned from. If you want to add a remote pointer to the repository of a collaborator, you may want to provide that collaborator’s username or a shortened nickname for the shortname.
  
### 4. **Create Branch (for your code)**
  - It's recommended to create a separate branch to submit your code.
  - It helps not to crash main code on main/master branch.
  - First, choose the issue that you can solve (recommended good-first-issues).
  - Comment on issue to assign, after assigning then create branch.  
  - It's Best practice to name branch as issue name and issue no together.
  - Type the following *git checkout* or *git switch* command on terminal 
  
  -> old way:
```
git checkout -b <new-branch-name>
```
  -> new way: It creates and switch to that new branch
```
git switch -c <new-branch-name>
```
  - replace <new-branch-name> with your branch name like issue-name-issue-no.
  
### 5. **Do Coding/Changes (Coding Time)**
  - It's Step in which you fix the issue or work on assigned issue.
  - It's the step in which you code to make project better.
  - It's the major part to solve the issues. So do it.
  
### 6. **Commit Changes (Save your code)**
  - After fixing an issue, you have to commit.
  - Commit should be atomic, means must contain solution of one particular issue.
  - Type the following *git commit* comand on terminal
  
```
git add .
```
```
git commit -m "A good commit message that describes the changes you've made."
```
  
### 7. **Update Forked Repo in GitHub(fetch update code if any)**
  - It's important to Update your forked repo with latest code from original one.
  - It's recommended to update before pushing code to avoid merge conflicts.
  
### 8. **Pull Updated / Latest Code (fetching latest code from forked repo if any)**
  - Fetching updated/latest code from updated forked repo.
  - If there is any new code that will be pulled to your local machine.
  - Type the following *git pull* command on terminal
  
```
git pull upstream main
```
  
### 9. **Push Code to Github (pushing your code to forked repo)**
  - Now, Push the code to forked repo under your account.
  - Type the following *git push* command on terminal
```
git push --set-upstream origin <new-branch-name>
```  
  - replace new-branch-name with your branch name.
  
### 10. **Create a Pull Request (request the owner to pull your code)**
  - To create Pull Request (PR), you have get the link from previous command result.
  - Go to that link or simply go to original repo.
  - There will be a automatic popup to create new pull request, click on that.
  - fill out the description of PR with neccesary details like 
    -> which issue you solved 
    -> what have you done output with screenshot
    -> that helps owner/maintainer to review your PR.

### 11. **Why wait until PR is merged (Keep Coding)**
  - Owner review your pull request(PR) and give feedback to make some changes or simply merge it.
  - Meanwhile, you can find another issue that you can solve.
  - Just comment on that to assign issue. 
  - After assigning issue, you can start work on that.

---
## Contribute Again? (follow the steps below)
---

### 12. **Update Forked Repo in GitHub (fetch update code if any)**
  - It's important to Update your forked repo with latest code from original one.
  - It's recommended to update before pushing code to avoid merge conflicts.
  
### 13. **Create new branch (for your another code)**
  - Create new brancg for another issue
  
### 14. **Repeat Step 5 and Step 6 (Code and Commit)**
### 15. **Update Forked Repo in GitHub (fetch update code if any)**
  - It's important to Update your forked repo with latest code from original one.
  - It's recommended to update before pushing code to avoid merge conflicts.
  - 
### 16. **Repeat Step 8, Step 9 and Step 10 (Pull, Push the code and make PR)**
  - Pull code to update code on local machine.
  - Push your code to forked repo on GitHub.
  - And finally make Pull Request (PR).

---
## Contribute More? 
---
### 17. **Repeat Step 12 to Step 16 (to keep contributing to the project)**
  - Repeating the Step from 12 to 16 is the work flow to contribute.
  - You also can do it same to contribute in any other project.

---

