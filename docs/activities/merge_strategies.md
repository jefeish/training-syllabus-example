## Begin the rebase

1. Switch to the rebase-me branch: 

```git
git switch rebase-me
```

2. Start the merge: 

```git
git rebase -i main
```

3. Your text editor will open, allowing you to see the commits to be rebased.
4. Save and close the rebase-todo.
5. Watch your rebase happen on the command line.
6. Take another look at your history: 

```git
git log --oneline --graph --decorate --all
```

7. If you merged now, it would be a fast-forward merge.
8. Finish the Merge
9. Switch to main, the branch you will merge into: 

```git
git switch main
```

10. Merge your changes in to main: 

```git
git merge rebase-me
```

---

## Setup to rebase

1. Find the SHA of the initial commit: 

    ```git
    git log --oneline
    ```

2. Reset to the SHA of the initial commit: 

    ```git
    git reset --hard SHA
    ```

3. Create a new branch and check out to it: 

    ```git
    git switch -c rebase-me
    ```

4. Cherry-pick files 4-6 onto the rebase-me branch using the reflog.
5. Switch to main: 

    ```git
    git switch main
    ```

6. Cherry-pick files 1-3 onto the main branch using the reflog.
7. Look at your history: 

    ```git
    git log --oneline --graph --decorate --all
    ```

8. If you merged now, it would be a recursive merge.
