# Readme for Information Retrieval System which is named SearchEngine

## PreProcessing( Part 1)

For preprocessing step a java file PreProcessing.java was created and it has a split method to split all the different documents in the 
cranfield collection into 1400 separate documents and then save them as txt files. The other one is in the main of the PreProcessing class 
which processes the broken down documents by removing all characters other than words and alphabets, removing all stopwords and also stemming 
the text. To test it yourself, just compile and run the PreProcessing class simply. Though you will need to create two folders in same folder 
where java classes are present namely "splitdoc" and "stemmeddoc" which have been created so that the files are arranged. An output file 
containing the length of the documents is also made.

## Information Retrieval( Part 2)

For this purpose, a java class PageEntry was created that inputs a documents and breaks it down into words and the words are stored in a 
HashMap and then calculated the IDF and WordFrequency in a document. Then a MySort class was created to sort the result to show top 100 results
only. To test this part simply run the SearchEngine class and input query messages on terminal. The output it produces are stored in text files
named query#.txt, where # is the query number starting from 0. For this part too you need to create a folder in the same location where the 
java classes are present names "queryOutputs" which will contain all the output query text documents. The output will also be printed to the 
terminal. Also, one thing to notice, you don't to run part1 again for part2 but you need to copy the folder "stemmeddoc" from part1 to the code
location of part2.

## IMPORTANT THINGS :

1)If you are using a mac os machine just copy past the both the folders to desktop you will not need to change the path for mac OS.
2)If you are using different OS then you have to change path in 5 places which is in part1 folder in PreProcessing file.
(Which are line no 23(to read the corpse), line no 30, line no 60, line no 65, line no 66-(to get the output)). make sure you store the output 
in a folder because you will get 1400 text files as output otherwise you might get messed up.
3)In part2 you have to change path in two file which are SearchEngine to output the text (line no 100) and second PageEntry(line no. 21) 
to read the output file which will be given by part1 program

## Steps to excute the program :

1)step 1 : There will be two folders "part1" and "part2" save both the folders on desktop
2)Step 2 : Go inside part1 folder you will see two folders "splitdoc" and "stemmeddoc", there will be two java files PreProcessing.java and 
Stremmer.java also you will find the corpse inside the part1 folder.
3)Step 3 : Go to terminal change the path to desktop and then go inside part1 folder, compile all the java files and run the PreProcessing 
program and wait. There will be atxt file which will give length of the all the 1400 documents and you will also find that the splitdoc will 
contain 1400 text file which will contain all the documents separatly also in another folder "stemmeddoc" you will find 1400 text file which 
are stemmed.
4)Step 4 : Copy this "stemmeddoc" folder in part2 folder. (Please read the folder which contains 1400 text files).
5)Step 5 : Change the path in terminal to part2 folder there are total 12 java files and 2 folder which are "queryOutputs" and "stemmeddoc" which
you copied from the output of part1.
6)Step 6 : Compile all the java files and run the SearchEngine file once you do it then you have to enter any query you want and that will give 
you an output, the output will be printed in terminal and will also generate a txt file in the folder "queryOutputs". Once you get an output you
can type another query as much as you want. to exit the program type "quit" in terminal
7)Step 7 : ENJOY!!!!
