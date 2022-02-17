## Merge Pull Request 

1. Navigate to your Pull Request (HINT: Use the Author or Assignee drop downs to find your Pull Request quickly)
1. Click **Conversation**
1. Scroll to the bottom of the Pull Request and click the **Merge pull request** button
1. Click **Confirm merge**
1. Click **Delete branch**

### Update local repo

1. Start by switching back to your default branch: **`git switch main`**
1. Retrieve all of the changes from GitHub: **`git pull`**

---

## CleaningUp the unneeded Branches

```git
git branch --all
git branch --merged
git branch -d <branch-name>
git branch --all
git pull --prune 
git config --global fetch.prune true
```
