
## 1
  * log into ieng6
 
(key_pressed) > `ssh ieng6` , <Enter>

  | then we will see the "password:", and after entered the password we will see

  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/login.png)

## 2
  * Clone your fork of the repository from your Github account
  
(key_pressed) > 'git clone <github_respository_URL>', <Enter>
  

  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/git_clone.png)
  
## 3
  * Run the test, domonstrating that they fail
  
(key_pressed) > 'cd lab7/', 'bash test.sh'
  
  | First, we change the working directory, then we run the test file
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/test1.png)
  
## 4
  * Edit the code file to fix the failing test
  
 (key_pressed) > 'vim ListExample.java', <Enter>
  
  | below image was before <Enter>
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/vim.png)
  
  |below image was after <Enter>
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/after_vim.png)

  
 (key_pressed) >  <:>, <$>, <->, <6>, <Enter>
  
  | Goes to 6th line from bottom
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/G.png)
  
 (key_pressed) >  <e>
  
  | Goes to the last letter of next word
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/e.png)

  
 (key_pressed) >  <r>, <2>
  
  | replace the current letter with 2
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/r2.png)

  
 (key_pressed) >  <:>, <w>, <q>, <Enter>
  
  | save and quit, below image was before <Enter>
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/wq.png)
  
  | below image was after <Enter>
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/after_wq.png)
  
## 5
  * Run the tests, demonstrating that they now succeed
  
  (key_pressed) > 'bash test.sh'
  
   ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/test2.png)
  
## 6
  * Commit and push the resulting change to your Github account
  
  (key_pressed) > 'git init', <Enter>, 
                  > 'git add ListExample.java', <Enter>,  'git commit -m "comment" ', <Enter>, 'git remote add origin <URL>', <Enter>
                  > 'git push origin main', <Enter>, <t>,<e>,<n>,<g>,<f>,<o>,<n>,<g>,<L>,<e>,<e>, <Enter>, <control+v>, <Enter>
  
  | Notice! I already do the 'git remote add origin' before this screenshot, so I use 'git remote show origin' to make sure I got
    | right URL, and the password is API key (which is the part of control+v) if you are using OSS login system 
      |(got to websit to generate one)
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/git_push2.0.png)

  
  



  
  
  
  
  
  

  


