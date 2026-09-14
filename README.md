# URC-CAD

This repository contains the official CAD files for the **Stony Brook Robotics Team (SBRT)** robot in the University Rover Challenge. Our robot is designed using Solidworks.

## How To Access

1. Clone repository onto your computer.
     
   You can do this by opening a terminal in the folder you wish to work in and running the following line
   ```bash
   git clone https://github.com/sbroboticsteam/URC-CAD
   ```
2. Install git large file system inside your repository
    
    ```bash
     git lfs install
    ```
3. Now you can access the CAD in Solidworks

## What To Do Before Each CAD Session 
1. Open a terminal in the URC-CAD repository folder
2. Run the following to check if there are any unstaged changes.  
    ```bash
       git status
    ```
   If there are changes, run this line. This will reset your CAD to the current working version.  
    ```bash
       git reset --hard origin/main
    ```
   
   If it does not list any changes, feel free to move ahead

3. Run: git switch main
4. Run: git pull origin main
5. Run: git lfs pull origin main
6. Create a new branch by running the following: git switch -c "subsystem name"/"what you're doing" (Ex. git switch -c arm/update-wrist-bracket)
7. Once again, run "git status" to make sure everything is peachy
8. Open up SolidWorks and start CADing

## What To Do After Each CAD Session
1. Open your terminal in the URC-CAD repository folder again
2. Run: git add .
3. Run: git commit -m "Brief overview of what you did"     (Ex: git commit -m "Update wrist bracket mounting geometry")
4. Run: git push -u origin <branch name> (Ex: git push -u origin arm/update-wrist-bracket)
5. Open the github repository web page and navigate to pull requests


## Collaboration Guidelines

- Pull the latest version before editing or adding new files.
- Make sure to not have Solidworks open when working with github 
- Create a pull request with your work after each CADing session
- DO NOT EDIT FILES THAT SOMEONE ELSE IS WORKING ON PLEASE (We are not fixing CAD merge conflicts lol)
- Coordinate with other subsystem teams when modifying assemblies.
- Contact the project leads if you have questions about workflow.
