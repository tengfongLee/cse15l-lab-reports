
# Lab Report 2

* ## _Part 1_
  
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


  
  * ## _Part 2_


  * Failure-inducing Input:


    ```
    public class ArrayTests{
      @Test
      public void testReverseInPlace(){
        int[] input1 = {3,2,1,4};
        ArrayExamples.reverseInPlace(input1);
        assertArrayEquals(new int[]{4,1,2,3}, input1);
      }
    }
    ```

  
  * Symptoms:


    ![Image](https://tengfonglee.github.io/cse15l-lab-reports/lab2/photo/ReverseInPlace_symptoms.png)

  
  
  * The Bug:
  
    ```
    static void reverseInPlace(int[] arr){
      for(int i = 0 ; i< arr.length ; i +=1){
        arr[i]=arr[arr.length - i - 1];
      }
    }
    ```

  
  * Bug Fixed:
  the arr.length have to be arr.length/2 in order to reverse correctly, which means when we use arr.length as for loop length we will result tw time     reverse in place which did not hcange anything, so we should chagne the loop body to
  ```
    temp = arr[i];
    arr[i] = arr[arr.length - i -1];
    arr[arr.length - i -1]=temp;
  ```
  This provide us a temp to store in order to avoid the overwrite
  
  Since the bug in the original code was the restriction of i and the body of foor-loop cause overwrite by the second half of the array which cuase        the array be reversed twice and overwrite after the method run.
  In conclusion, we change the restriction of the for-loop index i for array now the loop with loop properly without over looping(which aviod the problem that reverse array for twice), and create a reference variable to switch two index-symetric element in the array, this help us to aviod the overwrite issue, and this also help us to reduce the run time of the loop since we only need the traiverse half of the array(O(N/2)).


  * ## _Part 3_

  Acutally there is lot of stuffs that I haven't encounter beore, something like handle URL & Servers & remote control servers are new experience for me. 


