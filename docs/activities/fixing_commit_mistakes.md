## Reset Mixed

1. Once again, we will start by viewing the history of our project: 

    ```git
    git log --oneline
    ```

2. Go back one commit in history:

    ```git
    git reset HEAD~
    ```

3. See where the tip of the branch is pointing: 

    ```git
    git log --oneline --decorate
    ```

4. The changes we made in the last commit have been moved back to the working directory: 

    ```git
    git status
    ```

5. All the files still exist locally: 

    ```git
    ls
    ```

6. Move the files to the staging area before we can commit them: 

    ```git
    git add file5.md file6.md
    ```

7. Re-commit the files: 

    ```git
    git commit -m "re-add file 5 and 6"
    ```
    
---
    
## Revising your last commit

1. Create a new file:
 
    **Bash** 
    ```powershell
    touch file7.md
    ```

    **PowerShell**
        ```powershell
        Out-File file7.md
        ```
2. When you are adding files to the previous commit, they should be in the staging area. Move your file to the staging area: 

    ```git
    git add file7.md
    git commit --amend
    ```

3. The text editor will open, allowing you to edit your commit message.
