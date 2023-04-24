
# Lab Report 3

## Part 1
After writing a webserver called Stringserver, (using the server `port 6070`), to add words to
list use the format `/add-message?s=<string>` then to search use `/search?s=<string>`. 

![Image](https://raw.githubusercontent.com/viviantran706/cse15l-lab-reports/main/Screenshot%202023-04-23%20153543.png)
For the picture above the method that was used was the handleRequest and the Server method. The argument that it passed was the '/' which is why the page has thoes words. But some of the values includes array string that is empty, URI is http://localhost:6070/.

Adding `/add-message?s=Hello` after after `localhost:<server port>`,

![Image](https://github.com/viviantran706/cse15l-lab-reports/blob/main/Screenshot%202023-04-23%20153557.png)


To check what is on the list add `/search?s=Hello`, and this is your page should look:
![Image](https://github.com/viviantran706/cse15l-lab-reports/blob/main/Screenshot%202023-04-23%20153614.png)

After doing the same process to add *How are you* to the list, I did `/search?s=H` and the page should look like this:
![Image](https://github.com/viviantran706/cse15l-lab-reports/blob/main/Screenshot%202023-04-23%20153711.png)

The method that the code called for at this point was the handleRequest and the StringServer. The argument that this passes was the */search* and some of the values that are important is the contain empty string that returns the strings that contains the word that is searched. Then the returnSearch splits teh query to find what need to 
found (for this example it is anthing that contains h). Then str is an array that contained everything that was entered in the `/add-message?s=<string>`. With in this array it containes ' Hello '  and  ` How are you `.  Which is why this is printied on the page.



## Part 2

An input that does not induce failure: 
```public void testReverseInPlace() {
    int[] input1 = { 3 };
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 3 }, input1);
	}
 ```
A filure-inducing input:
```
public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```
![Image](https://github.com/viviantran706/cse15l-lab-reports/blob/main/Screenshot%202023-04-20%20123739.png)
```
The symptom is that the array was in the wrong order, and not reversed as intended
In the photo above we see that int he ReverseInPlace method failed one of the test which was the failure-inducing input, and it passes the first tester becuase it only contains one element

```
Before:
![Image](https://github.com/viviantran706/cse15l-lab-reports/blob/main/Screenshot%202023-04-23%20185324.png)

After:
![Image](https://github.com/viviantran706/cse15l-lab-reports/blob/main/Screenshot%202023-04-23%20185700.png)

## Part 3

From week 2 and 3, I have learned how a method that have the same out come has different bugs. 
For exmaple when looking at the reverseInplace method, when debugging there wa a few errors 
but if we looked at reversed method we see that the both have the same intentions, but each
had there own errors and bugs that were different. Another thing that I learned form these 
week was how to write tester cases. Beucase I have never wrote tester before with JUmit. So this
week was really useful.
