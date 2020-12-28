# Git Cheat Sheet

## **How to set up Git loacally**  


## Setting up you Name on git
Use the following to set up your first and last name:-  
```bash
git config --global user.name "First Last"
```
## Setting up your email on git
Use the following to set up your email:-
```bash
git config --global user.email "email@gmail.com"
```

## VSCode setup on your machine
_**NOTE:**_  
Everything below assumes you have _VSCode_ set up on your machine.  

Once set up you can use the command below to open VSCode from your command terminal:-
```bash
code
``` 

## Use VSCode as your git editor  

Once VSCode is set up you can use the following command to make git use VSCode as your primary git editor. The default git editor is Vim:-
```bash
git config --global core.editor "code --wait"
```
The "code" command opens VSCode editor, while the "--wait" command waits until the editor is closed before moving one the next instruction in the terminal.

## View your git config settings
Use the following command to view and edit your git config settings:-
```bash
git config --global -e
```

## Handling escape characters on Windows
Use the following:-
```bash
git config --global core.autocrlf true
```
## Handling escape characters on MacOS
Use the following:-
```bash
git config --global core.autocrlf input
```

# Setting Up a New Git Repo

## Initializing a new repo locally
First mkdir a new project folder then cd into it:
```bash
mkdir new_project_folder
cd "path/to/new_project_folder"
```
Then use the command to init git as a locla repo:-
```bash
git init
```
Then add your own README.md  
If your on windows use:
```bash
echo empty readme file  > README.md
```
If your on the Git Bash use:
```bash
touch README.md
```
Then add the files and commit them.
(Will be explained further later): 
```bash
git add -A
git commit -m "Initial Commit"
```
## Connect local Git to GitHub

You’ve now got a local git repository. You can use git locally, like that, if you want. But if you want the thing to have a home on github, do the following.

1. Go to github.
2. Log in to your account.
3. Click the new repository button in the top-right
     - You’ll have an option there to initialize the repository with a README file, but I don’t.
4. Click the “Create repository” button.  

Now, follow the second set of instructions, “Push an existing repository…”

```bash
git remote add origin https://github.com/vkuma/new-repo.git  

git push -u origin master
```

Love u
