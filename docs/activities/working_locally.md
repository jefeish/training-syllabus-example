## Create a local copy of the repo

1. Navigate to the **Code** tab of the class repository on GitHub.
1. Click Code -> **Clone or download**.
1. Copy the clone URL to your clipboard.
1. Open your command line application.
1. Retrieve a full copy of the repository from GitHub: **`git clone <CLONE-URL>`**
1. Once the clone is complete, cd into the new directory created by the clone operation: **`cd <REPOSITORY-NAME>`**

---

## Switching branches

```bash
git branch
git branch --all
git branch -a
git switch <BRANCH-NAME>
```

---

## Edit your file

1. Find your file, e.g **`05-USERNAME.md`**.
1. Open your file in your favorite text editor.
1. On line 6, replace the text with your caption.
1. Save your file.

 ---
 
 ## Make a commit
 
 ```bash
git status
git add my-file.md
git status
git commit -m “updating caption”
git status
```

---
 ## Push to GitHub
 
 ```bash
git push
```
