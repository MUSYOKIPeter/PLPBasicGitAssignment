# PLPBasicGitAssignment
PLP Software Engineering Week - Git &amp; GitHub Basics _ Hands-On Assignment: Basic Git And GitHub Workflow

Hands-On Assignment: Basic Git And GitHub Workflow
Objective: The objective of this assignment is to familiarize students with the basic workflow of creating a GitHub repository, connecting it to a local folder, and making commits and pushes.

Requirements:
- A GitHub account (create one if you don't have it already).
- Git installed on your local machine.
- A code editor of your choice (e.g., Visual Studio Code, Sublime Text).

Task 1: Repository Setup
1. GitHub Repository Creation:
- I logged in to my GitHub account.
- I created a new repository on GitHub (i.e., "PLPBasicGitAssignment").
- I initialized the new repository with a README file.

Task 2: Local Setup
2. Local Folder Setup:
- I created a new folder on my local machine and named it "PLPBasicGitAssignment".
- I opened a Terminal navigated to the created folder.
#I had initially saved the "PLPBasicGitAssignment" folder on "Documents". I however, could not access it as the change direction command resulted in a challenge as showcased by the Terminal: i.e., "PS C:\Windows\System32> cd /Users/musyo/documents/PLPBasicGitAssignment
Set-Location: Cannot find path 'C:\Users\musyo\documents\PLPBasicGitAssignment' because it does not exist."
#I therefore, opted to relocated the "PLPBasicGitAssignment" folder to "Downloads" and could then access it: i.e., "PS C:\Windows\System32> cd /Users/musyo/downloads/PLPBasicGitAssignment" 

3. Git Initialization:
- I initialized a new Git repository in my local folder through the commands:
(a) PS C:\Users\musyo\Downloads\PLPBasicGitAssignment> ls
(b) PS C:\Users\musyo\Downloads\PLPBasicGitAssignment> git init
    - Initialized empty Git repository in C:/Users/musyo/Downloads/PLPBasicGitAssignment/.git/

4. Connecting to GitHub:
- I linked my local repository to the GitHub repository I had created in Task 1 utilizing the commands: git remote add origin <repository-url>, i.e., 
(a) PS C:\Users\musyo\Downloads\PLPBasicGitAssignment> git remote add origin https://github.com/MUSYOKIPeter/PLPBasicGitAssignment.git

Task 3: Making Changes
5. Create a File:
- Inside my local folder, I created a new text file (e.g., `hello.txt`). I did this by opening Visual Studio Code, accessing the "PLPBasicGitAssignment" folder, then creating the text file.
- I added a simple text message (i.e., "Hello, Git!") on the 'hello.txt' file and pressed CTRL + S to save my progress.

6. Committing Changes:
- I stageed the changes by using the command "git add hello.txt": i.e., "PS C:\Users\musyo\Downloads\PLPBasicGitAssignment> git add hello.txt"
- I committed the changes by using the command "git commit -m "Add hello.txt with a greeting":, i.e., "PS C:\Users\musyo\Downloads\PLPBasicGitAssignment> git commit -m "Add hello.txt with a greeting"
#The following was the output: 
[master (root-commit) fbc61e8] Add hello.txt with a greeting
 1 file changed, 1 insertion(+)
 create mode 100644 hello.txt"

Task 4: Pushing to GitHub
7. Pushing to GitHub:
- I pushed the committed changes to my GitHub repository by using the command "git push -u origin master"
#The Module Instructore had requested Learners to utilize the command"git push -u origin main". However, I faced challenges as the Terminal gave the follwowing output:
PS C:\Users\musyo\Downloads\PLPBasicGitAssignment> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/MUSYOKIPeter/PLPBasicGitAssignment.git'

- Therefore, I was successfuly after running "git push -u origin master" since the output was as follows:
PS C:\Users\musyo\Downloads\PLPBasicGitAssignment> git push -u origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 257 bytes | 128.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/MUSYOKIPeter/PLPBasicGitAssignment/pull/new/master
remote:
To https://github.com/MUSYOKIPeter/PLPBasicGitAssignment.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.

Task 5: Verification
8. Verify on GitHub:
- I visited my GitHub repository in a web browser and confirmed that the `hello.txt` file and commit message were visible.

Submission:
- I ensured thaty all changes were pushed to my GitHub repository.
- I submit the link to my GitHub Repository through the LMS platform. 

