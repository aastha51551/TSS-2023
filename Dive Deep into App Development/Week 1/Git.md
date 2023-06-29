# Basic Git and GitHub

## What's Git?
Git is a distributed version control system (VCS) widely used in software development. It helps developers track changes made to their codebase, collaborate with teammates, and manage different versions of their projects. Git allows multiple developers to work on the same codebase simultaneously, merging their changes seamlessly and efficiently.Now, you may ask what's Version Control? Version control is a system that helps track and manage changes made to files and projects over time. It allows developers to keep a record of modifications, collaborate with others, and revert to previous versions if needed. 
## What's GitHub?
GitHub is a web-based platform that provides hosting services for Git repositories. It offers a robust set of features and tools that facilitate collaboration, version control, and project management for software development teams. GitHub serves as a central hub for developers to store, manage, and share their code with others.
## Installation
Follow the tutorial below to setup Git on your PC.
### [Git Installation Tutorial](https://www.linode.com/docs/development/version-control/how-to-install-git-on-linux-mac-and-windows/)
## Familiarizing Yourself with Git and GitHub
If you are completely new to this, here's a [video](https://youtu.be/PSJ63LULKHA) to help you out. Give this [article](https://www.hostinger.in/tutorials/basic-git-commands) a read to know about some basic git commands and their uses.
> **Note**
> It is essential to understand Git and GitHub as it will be your primary means to submit your assignments throughout this course. Also, it's knowledge is important if you are interested in working with open source projects in future.

### Initializing App Development project as Git repository and updating on GitHub:
To initialize an App Dev project as a Git repository and update it on GitHub using the command prompt, follow these steps:
* Create a new repository on GitHub: Go to [GitHub](https://github.com) and create a new repository. Take note of the repository URL.
* Open the command prompt or terminal on your computer.                                                                                      
 Navigate to the project directory: Use the cd command to navigate to the directory where your App Dev project is located. For example:     
  #### *cd C:\path\to\your\project*

* Initialize Git repository: Run the following command to initialize a Git repository in your project directory:                           
  #### *git init*

* Add files to the repository: Add all the files in your project directory to the Git repository using the following command:                 
  #### *git add .*

* Commit the changes: Create an initial commit for your project using the following command:                                                            
  #### *git commit -m "write name of this commit "*

* Add the remote repository: Link your local repository to the GitHub repository by adding a remote origin. Replace <repository-url> with the URL of your GitHub repository:
  #### *git remote add origin <repository-url>*

* Push the changes to GitHub: Push your local repository to GitHub using the following command. Note: If you are working with a different branch, replace master with the branch name.
  #### *git push -u origin master*

  You will have to enter login details of GitHub and its done!

  
