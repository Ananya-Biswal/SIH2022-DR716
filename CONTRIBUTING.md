## How to Contribute to this Project? (Git & Github Work Flow)

Contents:
1. [Fork the Repo](/CONTRIBUTING.md/#1-fork-the-repository)
2. [Clone Forked Repository](/CONTRIBUTING.md/#2-Clone-Forked-Repository)
3. [Configure remote](/CONTRIBUTING.md#3-configure-remote-upstream-to-original-repolink-forked-to-original-one---need-to-do-it-only-once)
4. [Create Branch](/CONTRIBUTING.md#4-create-branch-for-your-code)
5. [Make Changes/Code](/CONTRIBUTING.md#5-do-codingchanges-coding-time)
6. [Commit Changes/Code](/CONTRIBUTING.md#6-commit-changes-save-your-code)
7. [Update Forked Repo](/CONTRIBUTING.md#7-update-forked-repo-in-githubfetch-update-code-if-any)
8. [Pull Changes/Code](/CONTRIBUTING.md#8-pull-updated--latest-code-fetching-latest-code-from-forked-repo-if-any)
9. [Push Changes/Code](/CONTRIBUTING.md#9-push-code-to-github-pushing-your-code-to-forked-repo)
10. [Create Pull Request](/CONTRIBUTING.md#10-create-a-pull-request-request-the-owner-to-pull-your-code)
11. [Repeat again? then continue](/CONTRIBUTING.md#11-why-wait-until-pr-is-merged-keep-coding)

---
### 1. **Fork the Repository**
  - Click the fork button to fork the repository. 
  ![pic1 0](https://user-images.githubusercontent.com/65288518/156108901-c6ba0d91-168e-49e9-9c64-a36c5016617f.png)
  
  - It will make a copy of repository under your account. 
  ![pic1 1](https://user-images.githubusercontent.com/65288518/156108922-84f3f206-53f1-4593-b97c-20ffe90351e2.png)

  - Changes will not reflect in original one until pull request is merged by owner of the repository.
  
---  
### 2. **Clone Forked Repository**
  - Click on code button.
  - Select https or ssh (if ssh key is already setuped).
  - Click on copy icon.
  - ![pic2 0](https://user-images.githubusercontent.com/65288518/156108991-650aac10-4c0a-4a57-abe2-52db63fc595d.png)
  - Then, type the following *git clone* command in terminal to clone into your machine locally.
  
```
git clone "git@github.com:<your-username>/SIH2022-DR716.git"
```
 - replace <your-username> with your github username or basically just paste copied link in terminal.
 - ![pic2 1](https://user-images.githubusercontent.com/65288518/156109042-810346e9-b5a8-46ee-8191-60a8be2cf0a9.png)

---
### 3. **Configure remote upstream to original Repo(link forked to original one - *__need to do it only once__*)** 
  - This command links to the original repo (just do it once).
  - ![pic3](https://user-images.githubusercontent.com/65288518/156109096-47db1f41-b1e9-4bc0-9344-e2e94e5d9b3c.png)
  - Type the following *git remote* command on terminal
  
```
git remote add upstream git@github.com:Navdeepsingh4298/SIH2022-DR716.git
```  
  - In this example, 'upstream' is the shortname we have supplied for the remote repository since in terms of Git, "upstream" refers to the repository that you cloned from. If you want to add a remote pointer to the repository of a collaborator, you may want to provide that collaborator’s username or a shortened nickname for the shortname.

---
### 4. **Create Branch (for your code)**
  - It's recommended to create a separate branch to submit your code.
  - It helps not to crash main code on main/master branch.
  - First, choose the issue that you can solve (recommended good-first-issues).
  - Comment on issue to assign, after assigning then create branch.  
  - It's Best practice to name branch as issue name and issue no together.
  - ![pic4](https://user-images.githubusercontent.com/65288518/156109211-bdc30dc2-3170-4ba5-b637-bfaff8252686.jpg)
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

---  
### 5. **Do Coding/Changes (Coding Time)**
  - It's Step in which you fix the issue or work on assigned issue.
  - It's the step in which you code to make project better.
  - It's the major part to solve the issues. So do it.
  - ![pic5](https://user-images.githubusercontent.com/65288518/156109237-805dc746-21b1-4a88-ac62-6e3df9e7e6f8.png)
  - Above, it's just shown for the sake of demo. But you have to code in IDE of your choice.
  
---
### 6. **Commit Changes (Save your code)**
  - After fixing an issue, you have to commit.
  - Commit should be atomic, means must contain solution of one particular issue.
  - ![pic6](https://user-images.githubusercontent.com/65288518/156109382-c1619c88-72b3-469a-8f23-063ee4f1b533.png)
  - Type the following *git commit* comand on terminal
  
```
git add .
```
```
git commit -m "A good commit message that describes the changes you've made."
```

---  
### 7. **Update Forked Repo in GitHub(fetch update code if any)**
  - It's important to Update your forked repo with latest code from original one.
  - It's recommended to update before pushing code to avoid merge conflicts.
  - ![pic7 0](https://user-images.githubusercontent.com/65288518/156109794-deb71b9f-07d9-4c1a-9e92-e3c2d98d20e6.png)
  - ![pic7 1](https://user-images.githubusercontent.com/65288518/156109803-a63a4338-d0e8-42a6-bd03-5d473693c6f1.png)

---  
### 8. **Pull Updated / Latest Code (fetching latest code from forked repo if any)**
  - Fetching updated/latest code from updated forked repo.
  - If there is any new code that will be pulled to your local machine.
  - ![pic8](https://user-images.githubusercontent.com/65288518/156109833-27d73598-da3f-4a61-b178-e636307f1917.png)
  - Type the following *git pull* command on terminal  
  
```
git pull upstream main
```

---  
### 9. **Push Code to Github (pushing your code to forked repo)**
  - Now, Push the code to forked repo under your account.
  - ![pic9 0](https://user-images.githubusercontent.com/65288518/156109948-67220798-26ba-4faf-baa8-fe2a3c1d200b.jpg)
  - Type the following *git push* command on terminal
  
```
git push --set-upstream origin <new-branch-name>
```  
  - replace new-branch-name with your branch name.

---
### 10. **Create a Pull Request (request the owner to pull your code)**
  - To create Pull Request (PR), you have get the link from previous command result.
  - Go to that link or simply go to original repo.
  - There will be a automatic popup to create new pull request, click on that.
  - ![pic10 0](https://user-images.githubusercontent.com/65288518/156110064-efdefb37-2f86-4e60-a1e9-71fa03696e76.png)
  - fill out the description of PR with neccesary details like 
    * which issue you solved 
    * what have you done output with screenshot 
    * that helps owner/maintainer to review your PR. 
  - ![pic10 1](https://user-images.githubusercontent.com/65288518/156110091-35e7f101-a8af-47cb-846b-6119fa5405ee.jpg)
  - Then, PR will be listed in PR section like below:
  - ![pic10 2](https://user-images.githubusercontent.com/65288518/156110107-5ae75de3-f4cd-4173-b613-90d5f12effa2.png)

---  
### 11. **Why wait until PR is merged (Keep Coding)**
  - Owner review your pull request(PR) and give feedback to make some changes or simply merge it.
  - Meanwhile, you can find another issue that you can solve.
  - Just comment on that to assign issue. 
  - After assigning issue, you can start work on that.
  - But, When your PR is merged. Then, you can delete your branch for sake of cleaniness.
  - Deleting branch on your side won't affect code on original repo.
  - ![pic11 0](https://user-images.githubusercontent.com/65288518/156110408-07d4fe39-0e04-4eb6-990e-0be042ff1b76.png)
  - ![pic11 1](https://user-images.githubusercontent.com/65288518/156110416-4bae1f79-1d36-46cf-b32f-c6fd10851765.png)
  - Delete branch at local machine, Type the following command on terminal
  
```
git branch -d <branch-name>  
```  

---
## Wanna Contribute Again? (follow the steps below)
  
### 12. **Update Forked Repo in GitHub (fetch update code if any)**
  - It's important to Update your forked repo with latest code from original one.
  - It's recommended to update before pushing code to avoid merge conflicts.
  - ![pic12 0](https://user-images.githubusercontent.com/65288518/156110532-73aa579f-16cd-4814-adc2-09ea5813134c.png)
  - ![pic12 1](https://user-images.githubusercontent.com/65288518/156110550-f3270cdc-7a2d-4d33-b4f6-8987d6e428a3.png)

---  
### 13. **Create new branch (for your another code)**
  - Create new brancg for another issue
  - ![pic13](https://user-images.githubusercontent.com/65288518/156110585-e858e2af-51ac-4393-8314-0000113dfae3.jpg)

---  
### 14. **Repeat Step 5 and Step 6 (Code and Commit)**
  - Code the solution of issue. (again, i just make a file. but you have to solve the issue)
  - ![pic14 0](https://user-images.githubusercontent.com/65288518/156110646-52fc8957-be75-4f3e-80fb-a56f647f1116.png)
  - Commit your Code.
  - ![pic14 1](https://user-images.githubusercontent.com/65288518/156110632-aad3f4af-ba6b-4309-a628-5babdabdb260.png)

---  
### 15. **Update Forked Repo in GitHub (fetch update code if any)**
  - It's important to Update your forked repo with latest code from original one.
  - It's recommended to update before pushing code to avoid merge conflicts.
  - ![pic15 0](https://user-images.githubusercontent.com/65288518/156110751-b9e9b184-ff4f-4592-870a-3b410afcb735.png)
  - ![pic15 1](https://user-images.githubusercontent.com/65288518/156110780-766e374b-a806-4594-b8ca-5dae3ad221c4.png)

---
### 16. **Repeat Step 8, Step 9 and Step 10 (Pull, Push the code and make PR)**
  - Pull code to update code on local machine.
  -![pic16 0](https://user-images.githubusercontent.com/65288518/156110821-5abaedd3-b001-4e36-a0bc-b69fe651569a.png)
  - Push your code to forked repo on GitHub.
  - ![pic16 1](https://user-images.githubusercontent.com/65288518/156110843-4cfeaad6-4b51-4e37-999f-e1e56731b387.jpg)
  - And finally make Pull Request (PR).
  - ![pic16 2](https://user-images.githubusercontent.com/65288518/156110877-456a7194-3639-4c74-a4a0-9315564d0b9f.png)
  - ![pic16 3](https://user-images.githubusercontent.com/65288518/156110881-f27a63cc-25b1-4f66-bc4d-dd82ff10bf9f.jpg)
  - ![pic16 4](https://user-images.githubusercontent.com/65288518/156110888-bdcc1942-d212-4c1f-b2a0-c353bed10b21.png)
  
---  
## Wanna Contribute More? 
  
### 17. **Repeat Step 12 to Step 16 (to keep contributing to the project)**
  - Repeating the Step from 12 to 16 is the work flow to contribute.
  - You also can do the same to contribute in any other project.

---
