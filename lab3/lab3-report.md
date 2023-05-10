

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
  
    technical/government/About_LSC/CONFIG_STANDARDS.txt
    technical/government/About_LSC/Comments_on_semiannual.txt
    technical/government/About_LSC/ONTARIO_LEGAL_AID_SERIES.txt
    technical/government/About_LSC/Progress_report.txt
    technical/government/About_LSC/State_Planning_Special_Report.txt
    technical/government/About_LSC/Strategic_report.txt
    technical/government/Env_Prot_Agen/bill.txt
    technical/government/Env_Prot_Agen/jeffordslieberm.txt
    technical/government/Env_Prot_Agen/multi102902.txt
    technical/government/Env_Prot_Agen/tech_sectiong.txt
    technical/government/Gen_Account_Office/Testimony_cg00010t.txt
    technical/government/Gen_Account_Office/d01591sp.txt
    technical/government/Gen_Account_Office/gg96118.txt
    technical/government/Gen_Account_Office/og96014.txt
  
  
  
> ## Third command-line 'grep -i'

What does the command-line do?
  ignore uppercase vs lowercase.
Why it is useful?
  gerenlly speaking, it is useful because some time we want to ignore uppercase vs. lowercase. for example, sometime we want to looking for some word and it might be the beginning of the sentance.
  
  Example1_'-i'
  
  input
    
    grep -i "The system was blinking red" technical/911report/*
    
  output
    
    technical/911report/chapter-13.5.txt:            8 "The System Was Blinking Red"
    technical/911report/chapter-8.txt:            "THE SYSTEM WAS BLINKING RED"
    technical/911report/chapter-8.txt:            Tenet told us that in his world "the system was blinking red." By late July, Tenet
    technical/911report/chapter-8.txt:            As Tenet told us, "the system was blinking red" during the summer of 2001. Officials
    
    
  Example2_'-i'
  
  input
    
    grep -i "al qaeda aims at the american homeland" technical/911report/*
    
  output
  
    technical/911report/chapter-5.txt:            AL QAEDA AIMS AT THE AMERICAN HOMELAND
  
  
  
  
  
  
  
  
  
  
  
  
  
  
