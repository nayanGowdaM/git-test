# Git CLI

### Installation
[Install for here](https://www.atlassian.com/git/tutorials/install-git)

### Fundamenatls
* Version Check
    ```git
    git --version
    ```
* Using git help command 
    ```git 
    git help init //git help <command>
    
    git init -h   //Consise Help
    ```
* Configuring Username and Email
    ```git 
    git config --global user.name "xyz"
    git config --global user.email "xyz@exmp.com"
    ```

* Checking Your Current user name and passwords
    ```git 
    git config user.name
    git config user.email
    ```

* Checking your default git code editor
    ```git 
    git config core.editor
    ```
* Setting your default code editor 
    ```git 
    git config --global core.editor your_preferred_editor
    ```

### Creating a Local Repository
* Initializing Git local repo
    ```git
    mkdir repos
    cd repos
    mkdir myproj
    cd myproj
    git init
    ```
    Empty git repo has been initalized
    ```git
    ls -a
    . .. .git
    ```
### Comitting to Local Repo
* Checking status
    ```git 
    git status
    ```
* Stating Content
    ```git 
    git add file.txt
    ```
* Commit the Content
    ```git 
    git commit -m "file.txt" ```
* Viewing Commiting history
    ```git 
    git log
    git log --online   //Consise version of log commiting history
    ```
* For viewing git tree
    ```git 
    git log --oneline --graph
    ```

### Creating Repository
* Create your [github repo](https://github.com/)
* By clicking new repo with required info create a new github repo
* Using cli
    ```git 
    echo "# gitPractice" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin repolink.git
    git push -u origin main
    ```

### Push to a remote repo
* By initializing a local repo
    ```git 
    echo "# gitPractice" >> README.md
    git init
    git add README.md
    git commit -m "first commit"
    git branch -M main
    git remote add origin repolink.git
    git push -u origin main
    ```
* if initialized already
    ```
    git remote add origin git@github.com:nayanGowdaM/gitPractice.git
    git push -u origin main
    ```
* If you donot have a local repo them clone the github repo into your local system
    ```git 
    git add README.md
    git commit -m "commit file"
    git push -u origin main
    ```
### To know the remote repo name
```git 
git remote --v
```

### show Command
* Listing commit and git ids
    ```git 
    git log --oneline --graph
    ```
* Getting commit info using sha1 / git id of that commit
    ```git
        git show git_id_of that particular commit
    ```
* Referencing
    ```git 
    git show HEAD
    ```
    HEAD~n nth commit from HEAD
    HEAD^n nth parent for HEAD
    HEAD^^ 1st parent of 1st parent of HEAD

### Branching
* Listing the branches
    ```git
    git branch
    ```
* Creating a branch
    ```git
    git branch branch_name
    ```
* Checkout 
    * Based on Branch
        ```git
        git checkout branchname  
        ```
    * Based on commit or git/sha id
        ```git 
        git checkout commit
        ```
    * Deleting a branch 
        ```git 
        git branch -d branch_name
        ```