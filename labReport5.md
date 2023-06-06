# Lab report 5

## Part 1

```
What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?

Terminal, windows

Detail the symptom you're seeing. Be specific; include both what you're seeing and 
what you expected to see instead. Screenshots are great, copy-pasted terminal output 
is also great. Avoid saying “it doesn't work”.

From lab three, I cloned it onto my local desktop so when I ran it there were some 
symptoms and bugs that were seen in the code.  The error at the bottom shows where 
the error cam form. from this assignment I was expecting that I was bale to pass the 
test that were written. More specifically i was expecting it to return the list in a 
reversed way.



Detail the failure-inducing input and context. That might mean any or all of the 
command you're running, a test case, command-line arguments, working directory, 
even the last few commands you ran. Do your best to provide as much context as you can.



Some of the bugs that I think might be the cause for the symptoms is something to do 
with the for loop that was written, or a syntax error. Possibly a miss spell. But the 
list was returned as normal rather then flipped backward. 

```
1. TA response
  With the provided information above the bug is most likely the for loop. Since there
  there is an issue with it returning the loop as is. It looks like it might have been 
  flipped twices which would return the list as normal. Look further into the for loop that
  makes the method go through the whole list twice.
  
2. Student response and fixes


  ![Image](https://github.com/viviantran706/cse15l-lab-reports/blob/main/Screenshot%202023-06-05%20214839.png)
  
  
  I was able to look at the issue fo the for loop that loops through it twice, and I was able to 
  divde it by half so it would not change the second half of the list. Therefore I saw that when 
  it would change the first element with tthe last. I saw that it would then flip it back, the last
  then changing with the first elemtnt. Whcih reverses the effects that was wanted. Therefore by halfing
  elements that the for loops runs thorugh, the first half would flipped with the second half.
  
3. Extra information
  Files: 
  - ArrayExamples.java, Thihs is where the errors came form, There are two methods, reverseInplace ad reversed
  The main issue came from the reversedInPlace method. Both of then flips the list . The last method that was
  included in the file is averageWithoutLowest, which just takes out the loses and returns the average of the list
  not including tht lowest number
  - ArrayTests.java, THis is the test that were wrtten fo rht reversed methods, and where the ArrayExamples.java
  failes the test.
  - FileExample.java, There is one method that is called getFiles, and this gives all of the files that is under
  that directory.
  - LectureExamples.java, This was gone over in class and was the exmaple of the week, irrvelant to the issue.
  - LinkedListExample.java, this just intializes the valses for the Nodes, and has methods that allows
  to add to the begining of the node list, add to the end, get teh first wlwemnt, get teh last element, and turn it 
  string, then return the size fo the node list.
  - ListExamples.java, This had two methods, one of them returns a new list tthat has all the elemtns in the list which
  returns true and false if they are not the same. THe ther metnods just arranges the two list
  to be in a sorted list
  - MethodsTests.java, this is the test that werer written for the linkedlist file. 
  
  Commadn line that triggered the bug ` javac -cp ".;lib/hamcrest-core-1.3jar;lib/junit-1.13.2.jar" *.java`
  `java -cp ".;lib/junit-4.13.2.jar;lib/hamcrest-core-1.3.jar" org.junit.runner.JunitCore ArrayTests`
  
  
  When I fixed the issue, the list is now returned flipped which was the intented purpose of the method. 
  SO i chanegs the for loop to  i<arr.length/2 ; hwich fixed the issue of the mehtod going through it twice.
   


## Part 2
 Something that I have learned formt he second hal of this quater that I never knew about
 was the about how to grade with scripts. I really enjoyed this becuase it was fun seeing
 and programming it in fornt of us. Espcially the part where we can see how it worked after.
 Another this was using find and all of the commands lines that are possible. And how each
 of the ocmmands lines has their own benefits. Another thing that I enjoyed form my classmate
 was learning more about speicifc coding for this class. 
