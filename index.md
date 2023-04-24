# __Hello World__

## This is a tutorial on how to log into a course-specific account on ieng6:

> Step one: 
> * Set up your coding enviornment, most people prefer to use VScode. Linked [here](https://code.visualstudio.com/download).
> * You should see a page similar to the one below (Download the version based on your operating system.)
> * Once installed, open the application and proceed to step 2
> ![image](https://user-images.githubusercontent.com/130107248/230817817-c6c7ce4d-a953-4794-9d5a-5fd9c026c229.png)

>Step two: 
>* The next step is to work on logging in remotely, to do this you will need to know your course-specific [account information](https://sdacs.ucsd.edu/~icc/index.php)
>* The link will ask you to reset your password that you will then use to log in remotely.
>* The important part to note: Your user for your account should start with "cs15lsp23", the last 2 digits are specific to you (See image below)
>![image](https://user-images.githubusercontent.com/130107248/231019280-26531ef2-063b-4799-bcc2-9737f304c3bf.png)
>* Once you have this, open a new terminal which can be found by hovering over the top of the application. You should see something like this:
> > ![image](https://user-images.githubusercontent.com/130107248/234131991-c12b39c2-c086-4782-a99d-7bd5950c1e43.png)
<img width="1251" alt="image" src="https://user-images.githubusercontent.com/130107248/234132826-d42a223b-dbf7-45a2-976c-47b67f657b41.png">

>* In the bottom of the terminal to the far right, you should see a drop down arrow next to a plus sign. Here you will select "Bash" if you are a windows user. This menu is shown below
>![image](https://user-images.githubusercontent.com/130107248/234132225-34ce2621-5cca-4673-b4bf-79fe06636fe7.png)

>* This is where you will enter `ssh cs15lsp23__@ieng6.ucsd.edu` with the underscores replaced by your 2 digits found earlier
>* If this is your first time connecting to this server, it will ask if you want to continue. Select yes then enter your password created earlier 
> You should see this: (If you see this, move onto step 3)
> ![image](https://user-images.githubusercontent.com/130107248/231020571-011dc6db-8da4-4ffc-8725-f91826b33026.png) 

>Step three: 
>* Now we will get comfortable with running some commands (`cd`, `ls`, `pwd`, `mkdir`, and `cp`)
>* Type each command in the terminal
> > Try:
> > > * `pwd` This command will display the current working directory 
> > > * `cat /home/linux/ieng6/cs15lsp23/public/hello.txt` This command will print the contents of the path we provided
> > > * `ls -a` This command will list the files and folders of the path provided
> * continue to mess around with commands to get comfortable, you should see outcomes such as those pictured below when typing some of these commands
>![image](https://user-images.githubusercontent.com/130107248/234134558-e5ccdcef-df8c-4451-9357-0537dd634db1.png)
>Above you can see what is in our current working directory after we use the `pwd` command. Then we can see the contents of the "hello.txt" file which was "Hello!" which printed when we used the `cat` command. Finally, we ran the command `ls` which gives us different lists based on the paths provided. As you can see the commands `ls` and `ls -a` had differnt outputs. 
>
Once you are comfortable, you can log out of the remote server using CTRL-D
