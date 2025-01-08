# To create a github repository:

Create github account --> signin -->click on new --> create a repository --> give repository name --> give public/private access to that repo -->create repository.

# BRANCHING

Main branch - points to production.

Directly doing changes in the main branch it damages the whole system if any unwanted changes are done .Production environment gets disturbed
If there is any important file that has to be edited or modified. Generally we directly do not edit in the main file. Instead we create a copy of it , do the changes , carefully review the changs, if its okay then edit into the main file
In the same way we create another branch, do the chnages, test the changes, scan the changes, if everything is fine bring those changes into the main branch.This is called Branching . So Branching is very important and mandatory.
SHA CODE
It is a 40 character code. 
62487921f3843f6899bc97d47070a9c48c4c9244 (key)  our code (value)
1.If commit ID is changed, we can say that code is changed
2.If code is changed , commit ID is also changed.

# PULL REQUEST:

Someone has to review the changes before you merge the code into the main branch.

Workflow of pull request:

·  Create a branch: A developer creates a branch to work on a new feature, bug fix, or any other change.
·  Make changes: The developer makes the necessary code changes in that branch.
·  Push the branch: Once the changes are made, the developer pushes their branch to the remote repository (e.g., GitHub).
·  Open a pull request: The developer then opens a pull request, asking the repository maintainers or other developers to review and merge the changes into the main branch.
·  Review: Other team members examine the changes, suggest improvements, comment on the code, or approve the changes.
·  Merge: If the pull request is approved, the code changes are merged into the base branch, making them part of the main codebase.
·  Close/Delete: After merging, the pull request can be closed, and the feature branch can be deleted.

# Explanation with taking dosa example:

Create git-dosa repo. Add readme.MD file.

git add . ; git commit -m "Dosa project started first commit" ; git push origin main
No body is allowed to do changes in the main branch. We ve to protect the main branch.
We need to create some restrictions for main branch.
Go to settings

Give required/necessary rules for the main branch.
Create another branch from main branch-> do changes ->create pull request->get approval-> then merge the changes.
To get the commit ID
Git log
To create new branch
Git checkout -b plain-dosa

We ‘ve successfully completed plain dosa project needed to take it into the public. Need to merge with the main  branch.

Click on compare & pull request.
There are 4 commits in total.

The first is created newly. It was created by GIT not by us.
In order to get the changes into the main branch we use git pull command.
Merge commit will have 2 parent commits.
Merging preserves history, at any point you can track all the history of changes.
Merge commit is an extra commit created by GIT.
Creates a diamond history