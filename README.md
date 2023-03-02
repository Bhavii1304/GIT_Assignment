## GIT_Assignment

### 1. Pull and merge difference
    --> Example of pull request and two branch merge event.
- Create a feature1 branch and feature2 branch
- Pushed these branches on remote repository
- Create a pull request on Git hub
- By approving the pull request the feature branches merged with the main branch
### 2.  Rebase
    --> Try to rebase feature branch with master branch 

    git rebase main(This command is used for rebase)

- Create a feature branch named bugs
- Push bugs branch after commit
- To rebase this bugs branch with main branch use the command "git rebase main"

### 3. Change commit message

    --> Commit push on commit in feature branch and then change commit message

       git commit --amend -m "new message"(This command is used to change commit message)

- Create a branch named message 
- Make a commit with some message
- To change message of previous commit made use git commit --amend -m "new modified message"
- Push this commit to remote repository

### 4. cherry pick

    --> Pick some commits from feature branch to master branch 

       git cherry-pick <commit hash>  (This command is used to pick commits from feature branch to main branch)
  
- In a branch bugs make 2 commits 
- Pick one commit that want to add in main branch and copy its hash id using git log command
- Then using git cherry-pick <commit hash> command in main branch it pick that particular command from feature branch
- Push it on remote repository

### Drop commit

    --> Remove some commit from feature branch.
        git reset --hard HEAD^(This command is used to drop the last commit made in a branch) 
- Create a branch named tools
- Make 2 commits in it and push that on remote repository
- Using command git reset --hard HEAD^ drops the last commit     