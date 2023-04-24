
# Lab Report 2

* ## _First Part_
  
  >Here is my code for 'StringServer'
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab2/photo/code.png)
  
  >First input:
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab2/photo/first_input.png)
  
  ### ***Relevant Arguments:***
  
  * 'url ="http://localhost:1998/add-message?s=I%20do%20not%20believe%20this%20will%20work"'
  
  * 'stringStore ="I do not believe this will work\n"'
  
  * 'parameters={"s", "I%20do%20not%20believe%20this%20will%20work"}'
  
  ### ***Changes In Fields:***
  
  * 'url.getPath().contain()' means get the Path part of the URL and see if the path contains certain string by returning boolean variable
  
  * 'url.getQuery.split("=")' means get the Quert part of the URL and split by = if string contains one, it reference by the string array variable 'parameters'.
  
  *  Now stringStore equals to "I do not believe this will work\n"
 
  
  ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab2/photo/second_input.png)
  
  
  ### ***Relevant Arguments:***
  
  * 'url ="http://localhost:1998/add-message?s=It%20acutally%20works~~!!"'
  
  * 'stringStore ="I do not believe this will work\nIt acutally works~~!!\n"'
  
  * 'parameters={"s", "It%20acutally%20works~~!!"}'
  
  
   ### ***Changes In Fields:***
  
  * 'url.getPath().contain()' means get the Path part of the URL and see if the path contains certain string by returning boolean variable, which is differen than first input.
  
  * 'url.getQuery.split("=")' means get the Quert part of the URL and split by = if string contains one, it reference by the string array variable 'parameters'.(which is also split a differen string)
  
  * now stringStore equals to  "I do not believe this will work\nIt acutally works~~!!\n"
  
  
