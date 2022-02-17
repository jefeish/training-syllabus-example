## Git Bisect the long way

1. Initiate the binary search

  ```git
  git bisect start
  ```
 
7. Specify the commit where you noticed the code was broken

  ```git
  git bisect bad <SHA>
  ```

8. Specify the commit where you knew things were working

  ```git
  git bisect good <SHA>
  ```
  
11. Bisect will check you out to the midpoint between good and bad.
13. Run a test to see if the game would work at this point. Our test is to use ls to see if an index.html file exists.
14. If the game is still broken (there is no index.html file), type

  ```git
  git bisect bad.
  ```
  
16. If the game works (and there is an index.html file), type

  ```git
  git bisect good
  ```
  
18. Git will bisect again and wait for you to test. This will happen until Git has enough information to pinpoint the first bad commit.
19. When Git has detected the error, it will provide a message that SHA is the first bad commit.
20. Exit the bisect process

```git
git bisect reset
```

---

## Git Bisect the short way

```git 
git bisect start <bad-SHA> <good-SHA>
git bisect run ls index.html
git bisect reset
```

