Manual of creation "development" branch in git
1. Open your terminal and create directory for your project "new-project" with command: 
   mkdir new-project
2. Change current directory to your project directory "new-project":
   cd new-project
3. Initialize empty git repository:
   git init
4. Create file README.md
   nano README.md
5. Add file command prepares the specified files to be committed (in this example file README.md):
   git add README.md    
6. To commit changes into local repository whith message "init" run command:
   git commit -m "init"
7. Create new branch "development"
   git branch development
8. To switch on the branch "development" use command: 
   git checkout development
9. After changing local project use command from steps 5-6 to commit changes whith new message in current branch (on this step current branch is "development"):
   git add README.md 
   git commit -m "Added steps to manual"
10. Combine changes in "development" and "main" branches.
   git checkout main
   git merge development
11.Check status of your git with command:
   git status
12. To add edited project ot github use command:
   git remote add origin https://github.com/kvelen/new-project.git
   git push -u origin development
