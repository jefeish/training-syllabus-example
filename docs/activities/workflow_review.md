## Updating the README.md

```git
git clone URL
git switch -c readme-update
```

- Edit the URL in the README.md.
- Commit the changes to your branch.

  ```git
  git push -u origin readme-update
  ```
  
- Create a Pull Request in your repository (base: main, compare: readme-update)
- Merge your Pull Request.
- Delete the branch on GitHub.
- Update your local copy of the repository

  ```git
  git pull --prune
  ```
  
  ---
  
