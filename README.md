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

3. Run the following lines to update your CAD to the current working version
    ```bash
       git switch main
       git pull origin main
       git lfs pull origin main
    ```
    
4. Create a new branch by running the following:
    ```bash
       git switch -c "subsystem name"/"what you're doing" 
    ```
    Example: ```git switch -c arm/update-wrist-bracket```
   
5. Once again, run check the git status to make sure everything is peachy ```git status```
6. Open up SolidWorks and start CADing

## What To Do After Each CAD Session
1. Open your terminal in the URC-CAD repository folder again
2. Stage all of your changes and commit them to git
    ```bash
       git add .
       git commit -m "Brief overview of what you did"
    ```
    Example Commit: ```git commit -m "Update wrist bracket mounting geometry"```
3. Push your changes to the new branch you created at the start of your CAD session
    ```bash
       git push -u origin <branch name>
    ```
    Example: ```git push -u origin arm/update-wrist-bracket```
   
4. Open the github repository web page and click on the banner that says "compare & pull request"
5. Leave a brief description of your changes and then create a new pull request.
6. After that, you're free to log off and enjoy the rest of your day :D


## Collaboration Guidelines

- Pull the latest version before editing or adding new files.
- Make sure to not have Solidworks open when working with github 
- Create a pull request with your work after each CADing session
- DO NOT EDIT FILES THAT SOMEONE ELSE IS WORKING ON PLEASE (We are not fixing CAD merge conflicts lol)
- Coordinate with other subsystem teams when modifying assemblies.
- Contact the project leads if you have questions about workflow.
