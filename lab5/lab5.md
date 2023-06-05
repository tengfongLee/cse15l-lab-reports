
# Part1-Debugging Scenario

## Student Post:

  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab5/photo/1.png)
  
## SYMPTOM:

   ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/error_outout.png)
   
   ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/output.png)
   
   ### bash code:
   
   ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/sh1.png)
   
   
   ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/sh2.png)


   
## TA response

  In this case, you can see in the working direcory, grading-area, there is no ListTest in the folder. So, your guess is right
  
  something is wrong in the bashcode. As first image in bash code, we can see after copying the student submission into the grading-area 
  
  and changing the working directory we did not have any test file in the grading-area, and that's the reason casuing all the bug.
  
  In order to solve the problem, we can see even there is no test file in the working directory but we got one in _list-examples-grader-main_, 
  
  which was the working directory before 'cd grading-area', so we can move the file into grading-area by adding 'cp ListTester.java grading-area/'.
  
  Or simply move the ListTester.java into the grading-area directory will also work, but I suggest copy the file(this prevent moving file around).
  
  This should solve the proble hope this will help you :).
  
  
## Student screenshot after advice


 ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/after_fix.png)
 
 student response: Above image was the result after trying the change, which works perfect. 
 
 I think the bug was the direction of ListTester, which result the error that can't find ListTester. 
 
 This happend becasue I only changed the working directory, and forgot the ListTester was in somewhere else.

 And adding 'cp ListTester.java grading-area' before 'cd grading-area' slove the bugs.
 
## All the information needed about the setup including:

* The file & directory structure needed

![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/all_files.png)

* The contents of each file befoe fixing the bug

![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/sh1.png)

![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/sh2.png)

![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/java1.png)

![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/java2.png)

![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab4/photo/java3.png)

* The full command line you ran to trigger the bug

'bash grade.sh https://github.com/ucsd-cse15l-f22/list-methods-corrected'

* A description of what to edit to fix the bug

add 'cp ListTester.java grading-area/' befoe the line 'cd grading-area' in the grade.sh file


# Part2-Reflection

The coolest thing I learn is acutally build a simple auto-grader, which manage all kind of input into .txt and files. This includes 

bash command (shell) and Vim. Also, Github was good idea to take into class which is practical and useful.



