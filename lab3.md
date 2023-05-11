## Lab Report 3: JayLynne Redeaux 
#
__Command Researched: Grep & Source used: https://chat.openai.com

> __1: -c__
> * `grep -c "cell" technical/biomed/rr171.txt ` Output > `52`
>> The command -c is used here to look for all the occurances of the string "cell" in the given file and return a count of all the times it occured. This is useful when you want to compare frequencies of patterns of strings in files
>*`grep -c "emergency" technical/government/Alcohol_Problems/*txt ` Output > `technical/government/Alcohol_Problems/DraftRecom-PDF.txt:21
technical/government/Alcohol_Problems/Session2-PDF.txt:18
technical/government/Alcohol_Problems/Session3-PDF.txt:119
technical/government/Alcohol_Problems/Session4-PDF.txt:130 `
>> Another way to use this comand is to search through all the files ending in txt, this is helpful because it prints out all the files as well as the count right next to it

>__2: -v__
>* `grep -v "i" technical/government/Media/A_Perk_of_Age.txt ` Output > `By Kelly Greene
reach all 50 by the end of March. You have to pay the group's dues `
>> -v is useful when you want to get all of th elines that dont include a specific pattern or string. If you had a large sum of text and needed to filter out certain words in the lines this is the tool for you :P
>*
