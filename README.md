# Git Assignment - GibranAlvarez

a. What is an issue?
        Iitems created in a repository to plan, discuss and track work

b. What is a pull request?
        A proposal to merge a set of changes from one branch into another.

c. How do I open up a pull request?
        1. On GitHub on the pull request tab, in this repository it would be in the following URL: https://github.com/GibranAlvarez/git/pulls,
        2. then click on the green button called New Pull Request, 
        3. after that choose the base branch and the one with the changes, in this case they're base: "main" and compare: "assignment"
        4. clik on "Create pull request" green button
        5. Add a title for the PR and a Description of the changes made; in our cas for this DSI cours we need to answer 6 Questions. 
 
d. Give me a step by step guide on how to add someone to your repository.
   
    Method 1: 
	1. On GitHub got to your repository ex;  https://github.com/GibranAlvarez/git
	2. Click on the "Settings" tab on the top of the website, below  the   Username/repo_name
        3. Go to the "Access" > "Collaborators"  section on the left column on you browser
        4. Click on the Green button "Add people", you can choose/search typing or pasting their username, emails, name etc..
        5. Select one then click the green button "Add <user> to this repository" (<user> meaning the person you choose to add) 
        6. Enjoy xD
   
    Method 2:
	   You can use an api to add them in the terminal, in this case Simeon used a code in class which goes more or less like this
	   "" For username in $(cat usernames.txt); do
		gh api --method PUT "<URL for the repo>"
	      Done ""
	   Explanation: 
		What the api does is pass through each line on the text file with the usernames, 
		then run the api which adds each username to collaborators, 
		its an easier way if you have multiple users to add.
 
e. What is the difference between git and GitHub?
         GIT is an opensource version control tool and GitHub is a host service that stores git repositories	

f. What does git diff do?
         Show changes between commits 

g. What is the main branch?
         Is the default branch, it  receives all the accepted commits and merges and the one you, it used to be called "master"

h. Besides our initial commit if it is a new repository, should we directly push our changes directly into the main branch?
        No, commits should be pushed to a different branche from the main (good practice is making a branch for a specific task or change wanted), 
        once that branch is created and changes done then a Pull Request is needed to request that those changes are 
        added to the main branch. This is a better way to keep track of changes made without making any changes to the main branch.
        
        The way I see it is that the main branch has to always have "working" code (or at least the closest to the final prodcut), 
        and branches are a way to filtering changes and making sure that the main branch is always on a "working" condition. 
