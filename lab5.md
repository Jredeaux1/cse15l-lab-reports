__Part 1 – Debugging Scenario:__
> What enviornment are you using?: 
* I am using VsCode on my macbook (linux). I have a terminal open in vscode that I am running everything, I also go into vim to edit th efiles rather than opening them directly with vscode. 

> Detail the symptom you are seeing: 
* I am seeing a testTimedOutException when trying to fix the code in Vim. I edited the code to have "index2" instead of"index1" in ListExamples.java but I am still getting the error when trying to run the test. I am expecting to see all of my etsts passing like my peers but for some reason it is still failing. Below I have added my output and the error I am getting. 
* <img width="1762" alt="Screen Shot 2023-06-05 at 7 16 17 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/d404d51d-b900-47f0-aa14-9c6fb0f190a1">
> Detail Failure inducing context: 
> * The last few commands I ran: `ls` `cd lab7` and then I went into vim to edit the text file ListExamples.java. I used the down arrow till I got to the bug in the code which was the line " index1 +=1 ;" Shown in the image below are the lines I edited: 
> <img width="1771" alt="Screen Shot 2023-06-05 at 7 27 16 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/090162ee-42fd-4c4c-8fde-a772c90f6a13">
> The failure inducing input is `bash test.sh` 


1:  _Tutor Response:_ 
>* Hello! It would appear that the orginal code was changed beyond that one line, is there a reson you chose to add "system.out.println(result)"? Try changing the line back to the orginal code while keeping the changes to fix the bug, did that help? If that didnt help, try looking at the error you are getting. The error message indicates that the parser expected to find more code after line 46, but it reached the end of the file instead. This usually happens when there are incomplete statements or missing closing braces in the code above line 46. Go back through your code and ensure all of your brackets are there.

2: After fixing the brackets the student saw this in their terminal insinuating there was more than one bug in their code:
<img width="1792" alt="Screen Shot 2023-06-05 at 7 42 08 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/c1d77cd5-05ab-439d-9c22-a0b84fd95951">
The student reverted back to "return result" rather than "System.out.println(result)" and all the tests passed.
The bugs were that:
*1: The student had deleted the brackets causing the parser error
*2: The student didnt include a return statement and changed the code while trying to debug error 1 which they didnt revert back

The file & directory structure needed: Student used git clone https://github.com/ucsd-cse15l-s23/lab7 . Need to be cd into lab7 and in vim for ListExamples.java to see the code to edit. 
The contents of the file before fixing the bug: <img width="1771" alt="Screen Shot 2023-06-05 at 7 27 16 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/090162ee-42fd-4c4c-8fde-a772c90f6a13">
The full command line (or lines) you ran to trigger the bug: bash test.sh 


__Part 2 - Reflection:__
One of the cool things I had learned later in the quarter which I used for this lab report was using vim to acess and edit files. I am still not entirely sure if I prefer to use it rather than just opening the file because this was a mistake I had actually made, I didnt realize I removed the bracket and it was so hard to find where it was! I enjoy that Vscode shows where the error is which isnt provided in Vim but I do see why people use it as it is pretty efficient once you learn the tips and tricks. I liked the tutoring thing that we did in the lab, while i twas tedious it was helpful to learn some of the commands





