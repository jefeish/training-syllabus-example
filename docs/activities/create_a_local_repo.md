## Initialize a new local repository

1. Navigate to the directory where you will place your practice repo (`cd ..` to get back to the parent folder).
2. Create a new directory and initialize it as a git repository: 

    ```git
    git init practice-repo
    ```
    
3. CD into your new repository: 

    ```git
    cd practice-repo
    ```
    
4. Create an empty new file named `README.md`

    **Bash**

    ```bash
    touch `README.md`
    ```
    
    **PowerShell**

    ```powershell
    Out-File README.md
    ```
    
5. Add and commit the `README.md` file.

    **Bash**

    ```bash
    for d in {1..6}; do touch "file${d}.md"; git add "file${d}.md"; git commit -m "adding file ${d}"; done
    ```

    **PowerShell**

    ```powershell
    for ($d=1; $d -le 6; $d++) { Out-File file$d.md; git add file$d.md; git commit -m "adding file$d.md"; }
    ```
