## Lab Report 3: JayLynne Redeaux ❤️ 
#
Command Researched: __Grep__ 

> __1: -c__
> * Input: `grep -c "cell" technical/biomed/rr171.txt ` 
> * Output: `52`
> 
>> The command -c is used here to look for all the occurances of the string "cell" in the given file and return a count of all the times it occured. This is useful when you want to compare frequencies of patterns of strings in files

>* Input: `grep -c "emergency" technical/government/Alcohol_Problems/*txt ` 
>* Output: `technical/government/Alcohol_Problems/DraftRecom-PDF.txt:21
technical/government/Alcohol_Problems/Session2-PDF.txt:18
technical/government/Alcohol_Problems/Session3-PDF.txt:119
technical/government/Alcohol_Problems/Session4-PDF.txt:130 `

>> Another way to use this comand is to search through all the files ending in txt, this is helpful because it prints out all the files as well as the count right next to it

>__2: -v__
>* Input: `grep -v "i" technical/government/Media/A_Perk_of_Age.txt ` 
>* Output: `By Kelly Greene
reach all 50 by the end of March. You have to pay the group's dues `

>> -v is useful when you want to get all of the lines that dont include a specific pattern or string. If you had a large sum of text and needed to filter out certain words in the lines this is the tool for you :P
>> 
>* Input: `grep -v "emergency" technical/government/Alcohol_Problems/Session2-PDF.txt | grep -c "alcohol" ` 
>* Output: `93`

>> This command counts how many times the word "alcohol" appears in the file "Session2-PDF.txt", but only in lines that don't contain the word "emergency".This is another example of a way we can combine terms to help filter output.

>__3: -n__ 
>* Input: `grep -n "help" technical/government/Media/A_Perk_of_Age.txt ` 
>* Output: `13:provide self-help materials, and make referrals to legal aid
35:Another source of low-cost help also expanded this year: AARP's `

>> This command searches for the word "help" in the file "A_Perk_of_Age.txt" and displays each matching line along with the line number. The command -n is useful to find exactly where in the file a certain pattern or string is
>> 
>* Input: `grep -n "loosely" technical/government/Media/A_Perk_of_Age.txt > result.txt `
>* Output: [here](https://imgur.com/a/oZd92M3)
>>This command searches for the word "loosely" in the file "A_Perk_of_Age.txt" and saves the matching lines, along with their line numbers, into a new file called "result.txt".

>__4: -i__
>* Input: `grep -i "hElp" technical/911report/chapter-11.txt ` 
>* Output: `Ukraine, Belarus, and Kazakhstan; the Nunn-Lugar threat reduction program to help
            As for the Department of Defense, some officers in the Joint Staff were keen to help.` 
            
>>The "-i" option is useful because it makes grep case-insensitive, allowing it to match words regardless of whether they are in uppercase or lowercase letters.
>>
>* Input: `grep -i "fEDs" technical/government/Media/*txt ` 
>* Output: `technical/government/Media/Advocate_for_Poor.txt:all the paperwork. We got the nonprofit status from the feds. We`
>
>>This command searches for the word "fEDs" in any text file located in the "Media" directory within the "technical/government" directory, ignoring any case differences. This is important because you always need to know where the feds are hiding regardless of how they capitalize 😈 . 




Source used: https://chat.openai.com 🤖 (Prompt: Hey man, do me a solid and give me a bullet point list of 20 cool and helpful ways to use the grep command. Thanks) 
![image](https://github.com/Jredeaux1/cse15l-lab-reports/assets/130107248/83ba503d-4f31-461d-b145-733edeb589cf)
I took some of the bullet points along with the basic definition and implemented them in VSCode. I had to play around with them and figure out how they could be useful. I changed the output to fit into the folder we were given. 

