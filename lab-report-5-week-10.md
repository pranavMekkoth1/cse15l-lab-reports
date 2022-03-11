# Lab report 5 Week 10:

**Explain q1:**
- In Lab 9, the way that we found the diffrences between the implemtations was useing the `diff` command. For example, ` diff student-mdparse/results.txt markdown-parse/results.txt`
  This command would get the results from each of the implimentations then compare the results and show the tests that result in different outputs. I used a couple of the tests that resulted for this lab report.

**Test 1**
 - ![test 1 diff](https://user-images.githubusercontent.com/97641097/157922632-fde674dd-4f43-4203-a676-6f7b9d85c15c.png) Difference in test results for test 577.md
 - ![test](https://user-images.githubusercontent.com/97641097/157923326-fad44a3c-ee0e-42aa-8f57-5e49078dfc0c.png) test
 - I believe that only my implementaion output is correct. That is because as you can see from the screenshot of the expected result below, the expected output is an image and not a link. As such, since only my implemtation results in no links showing up as output, that means it is correct. The other implementation seems to indicate that the image is a link. 
 
 - ![expected](https://user-images.githubusercontent.com/97641097/157924538-4caafdb9-61ff-492c-b169-f40fd1d15086.png) Expected output
 - For the implementation that is incorrect, I believe the problem is that since images and links have very similar common mark format, and since there is no condition in the code to check for that difference, the the program reads the image as a link. The way that the program should be fixed is by including a new if statment in the markdown-parse.java file that checks for the exclamation point before the open bracket that indicates something is an image and not a link. In doing so, the result should be that there is no link in the test file.
 - ![image](https://user-images.githubusercontent.com/97641097/157925824-a4fc62df-53f6-4eda-ab7f-620579549297.png)                                            Here, in this snippet of joe's implementation (Which the implmentation we are finding differences with) adding a new if statment after line 69 (similar to what I described above) should fix the issue.

**Test 2**
- ![test2](https://user-images.githubusercontent.com/97641097/157926481-fe105c12-65db-4d0d-ab15-d2e86a88024c.png) Difference in test results for test 574.md
- ![test](https://user-images.githubusercontent.com/97641097/157927523-baa8778e-edc6-47fe-933d-3f4e673fb850.png) test
- For this test, I believe that only my implemtation output is correct. This is because , based on the expected output shown below, the result of the test should be an image with no links. My implemntation results in no links as outputs (as seen by the empty brackets). On the other hand, joe's implemntaion results in part of the text inside the brackets being displayed as a link. 
- ![expected](https://user-images.githubusercontent.com/97641097/157929436-df1927c2-6ce8-4d39-b03a-0c1c7583af36.png) Expected output
- For the implimentation that is incorrect, I believe that the problem is that the program reads internal links within the bracket portion of other links and/or images. I think that a good way to fix the issue is to include another if condition withing the program that negates any of the links that may appear within a set of open and close brackets. This way, even if a link format shows up within the format of other images and links, those internal links won't be read as links (just as shown in the expected output).
- ![image](https://user-images.githubusercontent.com/97641097/157925824-a4fc62df-53f6-4eda-ab7f-620579549297.png)                                            Here, in this snippet of joe's implementation adding a new if statment around line 66 (similar to what I described above) should fix the issue.
