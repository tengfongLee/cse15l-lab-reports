

# Lab Report 3

* Command: 'grep'

> ## First command-line 'grep -c'

What does the command-line do?
  This comment line count of matching lines only. 
Why it is useful?
  Assume we have a code file and I want to know how many instance did it create we can search for variable or object that we creat in order to know how memory space usage during run time. 
  Something like 'int', 'new' etc... or bying counting the key word we can konw which file we are looking without reading the content, ex, if A file only count the word 'UCSD' once, and B has
  many more compare to A than we know that file B has high chance that content are more relate to 'UCSD' which is what we looking for, this might save some time for us.
  
  Example1_'-c'
  
  input
  
    
    grep -c "KSM" technical/911report/chapter-1.txt
    
    
  output
  
    0

  Example2_'grep -c'
  
  input
  
   
    grep -c "KSM" technical/911report/chapter-5.txt 
   
    
  output
  
    130
    
    
   >KSM stand for Khalid Sheikh Mohammed which is a person's name, and since all the file in 911report are named by number, so it is hard for us to know which file is the one we want, and this is  one way for us to find out. This case might be extrem, but if we are looking for some word that is command see but more often in the file we want then this is a perfect fit commmand.


    
    

> ## Second command-line 'grep -l'

What does the command-line do?
  This command line output the matchiing file only
Why it is useful?
  We can using this command to find the file we want with a rare word, which is like person's name etc... . Combine with the pervious command-line will be able to find the file in more efficient way. If we are searching something with extremly common word we can use -l first to filter the file and use -c to see which one contain more word(which has higher chance to be what we're looking for)
  
  Example1_'-l'
  
  input
    
    grep -l "KSM" technical/911report/chapter-1.txt technical/911report/chapter-5.txt technical/911report/chapter-6.txt technical/911report/chapter-9.txt 
    
  output
    
    technical/911report/chapter-5.txt 
    
    
  Example2_'-l'
  
  input
    
    grep -l "2005" technical/government/*/*
    
  output
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
