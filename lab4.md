## __Lab Report 4: JayLynne Redeaux 🧠__
Step One: To log into ieng6 I typed `cs15lsp23kv@ieng6.ucsd.edu` then pressed `<enter>` since I previously set up my SSH key, I did not have to enter a password. The image below shows the screen when entering ieng6.
<img width="850" alt="Screen Shot 2023-05-22 at 9 04 04 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/57cc0089-fdd7-4117-a814-02daf9d37a7d">

Step Two: The next step is to clone the repository into my directory. I did this by doing `<command v>` which placed `git clone https://github.com/ucsd-cse15l-s23/lab7` into my terminal. From there is was important that  made sure the clone was sucessful, I did this by typing `ls` then changing my directory into lab7 using the command `cd lab7` as seen below. 
<img width="746" alt="Screen Shot 2023-05-22 at 9 26 47 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/e61ec75b-8570-4133-9826-3e605c1f071c">

Step 3: Prior to fixing the code, I made sure to run the test to make sure they are currently failing. I did this by tying `bash test.sh` into my command line followed by `<enter>` the output is shown below. 
<img width="691" alt="Screen Shot 2023-05-22 at 9 41 00 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/a84bb02a-002f-4e1c-89bb-2e00f118d48c">

Step 4: It is now time to fix this error, we have to go into vim first by typing `vim ListExamples.java` which opens up the editor. Keys pressed: `<down>` x47 `<left>` x3 once I got to the spot where I was hovering over the 1, I pressed `x` once to delete it. To go into insert mode and to edit: Keys pressed ~ `i` `2`. Finally, before testing if the edits worked. I saved my work. Keys pressed: `<esc> :wq! <enter>` . As you can see in the photo below, the changes have been saved. 
<img width="749" alt="Screen Shot 2023-05-22 at 9 48 57 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/b331e30e-d6b1-4f6b-a96d-999a4e9070a1">

Step 5: To test the changes, `<up><up><enter>`  command was 2 up in the search history, so I used up arrow to access it. As you can see in the image below,the tests ran sucessfully 

<img width="618" alt="Screen Shot 2023-05-22 at 9 51 37 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/c4b95cbd-63dc-4abd-9686-c3325121145a">

Finally, the last step 6: save all the work by commiting to main. I did this by typing `git commit ListExamples.java` which then opened another vim insert menu where I was able to type my message to go along with my commit. Once I was done typing I saved and exited doing `<esc>:wq!<enter>`

<img width="688" alt="Screen Shot 2023-05-22 at 9 58 11 PM" src="https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/5af7b61f-f0ee-44ca-b28b-9ed82f9fd0cf">



All done 🕺 
