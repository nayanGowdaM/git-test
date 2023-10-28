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