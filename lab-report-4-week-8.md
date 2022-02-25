# Lab Report 4 week 8
## by Pranav Mekkoth

[repository reviewed last week](https://github.com/ExtraExaByte/MarkDownParse)

[my repository](https://github.com/pranavMekkoth1/markdown-parse.git)

**Snippet 1**

 - Snippet expected result:

![What snippet should produce](https://user-images.githubusercontent.com/97641097/155671234-0408ddb1-c359-40bd-a299-653813d5d180.png)

  - Test:
   
   ![test1](https://user-images.githubusercontent.com/97641097/155672753-a217a59a-af9d-4bee-ae91-671246468232.png)
  - My code expected output:
   
   ![image](https://user-images.githubusercontent.com/97641097/155673807-e3106397-39f1-4ca4-ad8f-838642021099.png)
   
  - Reviewed MakdownParse output:
 
   ![image](https://user-images.githubusercontent.com/97641097/155675498-9f150e45-bce9-4057-b826-08dd1dd50b48.png)

**Snippet 2**

  - Snippet expected result:

  ![What snippet should produce](https://user-images.githubusercontent.com/97641097/155675882-65394d64-1ce3-4646-b776-ee6c9bbf9c26.png)

  - Test:
   
   ![test1](https://user-images.githubusercontent.com/97641097/155676407-d600655f-8d0a-4706-b0f0-431db5835721.png)
  - My code expected output:
   
   ![image](https://user-images.githubusercontent.com/97641097/155677151-dd0a5a34-507d-45bd-946c-5a77db0f467c.png)
   
  - Reviewed MakdownParse output:
 
   ![image](https://user-images.githubusercontent.com/97641097/155677241-7a96ad8b-5a54-4a54-b2ea-29c70dedb546.png)


**Snippet 3**

  - Snippet expected result:

  ![What snippet should produce](https://user-images.githubusercontent.com/97641097/155782161-4b8196f0-b262-4b09-b1a2-3eb01b9af26e.png)

  - Test:
   
   ![test1](https://user-images.githubusercontent.com/97641097/155678094-017c9a3f-0dc6-432f-ac85-409fd3c7a427.png)
  - My code expected output:
   
   ![image](https://user-images.githubusercontent.com/97641097/155678235-3ad75cac-ad73-487f-86f5-0f71950bd50f.png)
   
  - Reviewed MakdownParse output:
 
   ![image](https://user-images.githubusercontent.com/97641097/155678444-058a085c-5608-44fd-aa43-c95c0f5f54a0.png)
    
 **Lab Report Questions**
 
 - For snippet 1 shown in the lab report instructions, I do believe that there is a way to create a general fix that can be applied to the markdownParse.java file. I think that one way to solve it is by writing an if statement within the while loop of the getlinks method that only determines if it is a link if there is no character prior to the first open bracket and if there is an open bracket and then a close braket immediatly preceding the open parentheses regardless of if there is a second open or close braket between the 2. You would also need an additional if statement to include the inline text immedeatly after link as link text.

 - For snippet 2, I don't believe there is a relativley short way (<10 lines) to find a general fix that can be applied to fix the error. After applying the fix mentioned in the previous bullet point (to only read outer brackets), you would then need a condition that only reads the outermost parentheses as being the actual link. Then, you would also need a have to have a seperate if loop to check if an imbedded links (in its entirirty) is within a set of brackets (if so, only read the embedded link as a link). I beleive that putting all these conditions into markdownParse would exceed the 10 line limit. 

 - For snippet 3, I believe that a relativley short fix is possible. 

 
