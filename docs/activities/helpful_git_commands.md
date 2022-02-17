## Moving and renaming files with Git

1. Create a new branch named `slow-down`.
1. On line 9 of the `index.html` file, change the background url to `images/texture.jpg`.
1. On line 78, change the timing for the game to speed it up or slow it down.
1. Save your changes.
1. See what git is tracking

    ```git
    git status
    ```

6. Create a new, empty directory

    ```bash
    mkdir images
    ```
  
7. Move the texture file into the directory with git

    ```git
    git mv texture.jpg images/texture.jpg
    ```
    
---

## Staging chunks of changes

1. See what git is tracking

    ```git
    git status
    ```
    
2. Move some parts of some files to the staging area with the `--patch` flag:

    ```git
    git add -p
    ```

3. Stage the hunk related to the image move: `y`
4. Leave the hunk related to the speed change in the working area: `‘n’`
