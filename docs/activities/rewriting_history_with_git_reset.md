## Reset Soft

1. View the history of our project: 

    ```git
    git log --oneline --decorate
    ```

2. Identify the current location of HEAD.
3. Go back two commits in history: 

    ```git
    git reset --soft HEAD~2
    ```
    
4. See the tip of our branch (and HEAD) is now sitting two commits earlier than it was before: 

    ```git
    git log --oneline --decorate
    ```

5. The changes we made in the last two commits should be in the staging area:

    ```git
    git status
    ```

6. All the files still exist locally:

    ```bash
    ls
    ```
    
7. Let's remove the extra file we created earlier: 

    ```git
    git rm --cached file7.md
    ```

8. Now, we'll re-commit these changes without the extra file: 

    ```git
    git commit -m "re-add file 5 and 6"
    ```

---

## Reset Hard

1. Start by viewing the history of our project with: 

    ```git
    git log --oneline
    ```

2. Reset to the point in time where the only file that existed was the `README.md`: 

    ```git
    git reset --hard <SHA>
    ```

3. See that all of the commits are gone: 

    ```git 
    git log --oneline
    ```

4. Notice your working directory is clean: 

    ```git
    git status
    ```
        
5. See that the only files in your repository are the `README.md` and `file7.md`: 

    ```bash
    ls
    ```
