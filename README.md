New-Project: Git Setup Guide

This document provides the step-by-step instructions for initializing this repository's Git workflow. The primary goal is to create a development branch, add this README, and merge it safely into the main branch.

This guide fulfills the requirements for PROM-42164.

Step-by-Step Instructions

Follow these commands in your terminal from the root of the 'new-project' directory.

1. Create the 'development' Branch

First, create a new branch named development and switch to it. This is where you will do all new feature work.

# Create the new branch and switch to it in one command
git checkout -b development


(Expected Result: A new branch called "development" is created and you are switched to it successfully.)

2. Create and Stage the README.md

Now that you are on the development branch, create this README.md file.

After creating the file and adding this text, you must "stage" it (add it) to let Git know you want to track it.

# Add the README.md file to the staging area
git add README.md


(Expected Result: The "README.md" file is created, instructions are added, and the file is staged for commit.)

3. Commit the Changes

Commit the staged file to your development branch. This saves a snapshot of your work on this branch.

# Commit the file with a descriptive message
git commit -m "feat: Add setup instructions to README.md"


(Expected Result: The changes are committed to the "development" branch successfully.)

4. Merge 'development' into 'main'

With the work completed and saved on the development branch, you can now merge it into the main branch.

# First, switch back to the main branch
git checkout main

# Now, merge the changes from 'development' into your current branch (main)
git merge development


(Expected Result: The changes from the "development" branch are merged into the "main" branch successfully.)

5. Push All Changes to GitHub

Finally, push both of your local branches (main and development) to the remote GitHub repository (called origin) so your team can see them.

# Push the main branch
git push -u origin main

# Push the development branch
git push -u origin development


Setup Complete: The repository is now set up with a main branch and a separate development branch.
