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
git remote --verbose
```