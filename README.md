# labreport5
# cse15l-lab5-reports
----------------
**Researching Commands**


- Since I really liked this lab, I will do a researching command lab on another command option which is the command less this time.
 
 - less command allows you to view the content of a file, and it allows you to searche for specific content in the file and navigate the file as well. 
 
 - 1) -N
 The command line -N option is a kind of a command line option that displays each line number of the file being reviewed, moreover, if you just use the less command, it will display the file content but without numbers of each line. Basically, the -N command line in less command is a way to have the lines of a file numbered. 
 - For example, in the screenshot below, I will first only display the content of a file called WhereToMadrid and syntax to do so is 
 ```
 ayahsmacbook.@Ayahss-MacBook-Pro berlitz1 % less WhereToMadrid.txt
 
 ```
 
 - a) Using less command to view the ccontent of a file:
 
<img width="568" alt="image" src="https://user-images.githubusercontent.com/122571192/224853982-43eb5b82-a6c6-413d-b58c-915cf5c757ec.png">

 

 
  - b) Now using -N the command-line and its output Example 2: 
  - The syntax is: 
  ````
ayahsmacbook.@Ayahss-MacBook-Pro berlitz1 % less -N WhereToMadrid.txt
  ````
  - The output will be:
  
<img width="565" alt="image" src="https://user-images.githubusercontent.com/122571192/224854696-971b6dc3-4395-4526-a627-d26d38841b80.png">

  
- Here we can see the difference between the two examples, where on the first one the file was viewd without the line numbers. However, in the second example the file was viewd with the line numbers displayed of the file content. 
  
 - The -N option in the less command is very useful and helpful because it helps you to keep track on the comtent of large files. Especially, when dealing and debugging with large code files.
 


 - 2)" +(Number) or + (search word)" 
 - This command-line starts displaying the file from a specific line number or from a specific word the user wants to start from. The syntax for this command-line is.  

 
 
 - a) First example is starting from a specific line number in the text file, and the syntax to do so is: 
  
 ````  
  ayahsmacbook.@Ayahss-MacBook-Pro berlitz1 % less +20 WhereToMadrid.txt
 ````
- The output 
<img width="572" alt="image" src="https://user-images.githubusercontent.com/122571192/224857580-5ae4bc10-cccb-45b3-88a7-4060da3cd59f.png">
- Here the text file will be displayed from line number 20 which starts from the word Castile.



- b) Second example starting from the line that contains the first occurance word that is being searched. 
- The syntax to do so is: 
````
ayahsmacbook.@Ayahss-MacBook-Pro berlitz1 % less +/city WhereToMadrid.txt
````

- The output: 
<img width="574" alt="image" src="https://user-images.githubusercontent.com/122571192/224860548-3dfad93d-c6ab-4472-969d-e64a2c2dafe5.png">

Here the file will be displayed from the place where the word "city" first appeared in the text file. 
- This command-line is helpful becasue it helps us start the text file from a specific place. It is alos very useful in large files where if someone knows the word or the line they are searching for where this command will just save time by locating the file from that lineof word without having to scroll through the file or trying to find a string. Also, I found this interesting and helpful information from the lab tasks, and trying the command-line by myself, and chatGPT. 
 

- 3) -i
This command line -i option is a kind of a command line option that ignores the case sensitivity when searching for a pattern. This command line is helpful when searching for something in a file, and you want all the words in lower and upper case. Because this command line will not distinguish between uppercase and lowercase. 

- a) Here is an example of me trying to find where the word "SMALL" appeared in the WhereToMadrid text file. 


- The syntax to write the command was ```less -i WhereToMadrid.txt```, then after entering the file we will write /(the word we are trying to search).
- The ouput:
<img width="573" alt="image" src="https://user-images.githubusercontent.com/122571192/224864585-9ac05652-7722-4457-84a4-153ba3221256.png">
 Altough here the word "Small" appears to be in lowecase letters in the text file, however, I was still able to find it using the option of ignoring the case sensetivity. 

- b) The second example is trying to find the same word using the same command line, but i will use the option of taking case sensitivty in account. 
-The output:
a. First I made the case significant in searching for a word. 
<img width="358" alt="image" src="https://user-images.githubusercontent.com/122571192/224864994-54f80d9d-3ede-4ad2-aed0-ebf691d8cfe6.png">
b. Then I searched for the same word I searched previously ```/SMALL``` with capital letters. 
-The output: 
<img width="570" alt="image" src="https://user-images.githubusercontent.com/122571192/224865113-622a35f1-210b-4c32-9a10-d73670faf99c.png">

- When I make it sensitive for cases, it will not find the word small, altough we know it exists in the file from the last example, but since it is case sensitive it will only match the exact words. 
- This command-line is helpful because it helps you to quickly find a certain pattern in a file without having to go through the whole file line by line which again saves time and effort. Also, I found this interesting and helpful information from the lab tasks, and trying the command-line by myself, and chatGPT. 
 



- 4) -S
This command-line is an option with the less command, and it helps to view the very long lines that might be wrapped to multiple lines becuase they cannot fit in the width of the terminal window. 
- a) First Example, I am trying to view the text file WhereToMadrid whihc has longer lines that cannot fit in the width of my screen.
- First, the output of viewing the text file without using the -S command-line will be: 
<img width="506" alt="image" src="https://user-images.githubusercontent.com/122571192/224872258-7ecf412f-5f90-4cfd-b8a2-722a245fca77.png">

- The syntax for using the -S command-line is:  
`````
ayahsmacbook.@Ayahss-MacBook-Pro berlitz1 % less -S WhereToMadrid.txt
`````
- The output:
<img width="507" alt="image" src="https://user-images.githubusercontent.com/122571192/224872334-08bfd655-d626-4148-a9e8-e3cc8f1d9579.png">

  
- b) Second example I tried the same command-line with a different text file. 
- Syntax:
`````
ayahsmacbook.@Ayahss-MacBook-Pro berlitz1 % less -S WhereToJapan.txt

`````
The output:
<img width="503" alt="image" src="https://user-images.githubusercontent.com/122571192/224872465-75b2c5c7-ab63-4023-90d6-71d652a17c71.png">

- We can see the difference between reviewing the text files with the -S command-line and without. When we do not use it, the texts seem to be unorganized, and it is displayed in a confusing way. However, when we did use the -S command-line, the text got more organized and it order for us to see the rest of the text file we can use the arrows as it appears on the terminal. 

- The -S command-line is helpful if you are trying to read long files, and it makes the files look more organized and fit your terminal width window where the lines will not be cut in the middle. It provides a clearer way when we look at the files which can also help saving time when reading a more organized file. 
 


 
 
 


