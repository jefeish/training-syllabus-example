## Cherry-pick a commit

1. Find the commit ID where you added `file4.md`: 

    ```git
    git reflog
    ```

3. Cherry-pick that commit: 

    ```git
    git cherry-pick <SHA>
    ```
    
---

## Directional reset

1. View the history of everywhere HEAD has pointed: 

    ```git
    git reflog
    ```

2. Reset to the point in time where the original `file6.md` was created: 

    ```git
    git reset --hard <SHA>
    ```

3. See your restored history: 

    ```git
    git log --oneline
    ```
