## Protected Branches

1. Select the **Settings** tab.
1. Select **Branches** from the menu on the left side of the screen.
1. Click the **Add rule** button next to Branch protection rules.
1. In the Apply rule to textbox type the name of the branch you would like to protect, for example,` main`.
1. Click the **`Create`** button.

---

## Create a CODEOWNERS file

1. Go to the **Code** tab of your repository.
1. Click the **Create new file** button.
1. In the `Name your file...` textbox enter **`CODEOWNERS`** (no extension necessary). You can add this to a **`.github/`** directory if desired by entering **`.github/CODEOWNERS.`**
1. On the first line, type **`*          @YOUR_USERNAME`**
   - This means that you will be the default owner for everything in the repo, unless a later match takes preference.
1. On the next line, type **`*.js       @GITHUBTEACHER`**
   - Order is important. The last matching pattern for a given change takes precedence.
1. Scroll down, and type a commit message into the Commit new file dialog box.
1. Click the **Commit** new file button to save your changes.
1. Now that you have created a **`CODEOWNERS`** file, go back to your branch protection settings and click the **Edit** button next to main.
1. Under Rule settings, select the option to **Require pull request reviews before merging** and Require review from Code Owners. Remember to click Save changes.
