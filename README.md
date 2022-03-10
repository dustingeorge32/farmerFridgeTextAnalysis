# farmerFridgeTextAnalysis
Coding Assessment Farmer Fridge Dustin George 3/11/2022


#Overview of Solution

##Step 1 Reading the File##

When it comes to text analysis the programming language I wanted to utilize was Python due to its ability to parse text easier than other languages and the easy to use dictionaries (to keep track of word frequencies). 


First step is to create a function that is able to read a text file from an input. By default, if there is no text file then the exercisedocument.txt file will run that way we are parsing some sort of file.


After, the text file we need inputs from the user on whether to exclude stop words, consider stem words, top results desired (fun little exercise for myself) and if they use stop words a file that contains the stem words so that can be used.


If the user wants to use stop words then we must read the file that contains the stop words and use a set to store all the words that are considered stop words and store that into a set variable.


##Step 2 Writing to the dictionary/keeping track of word frequency##


When reading the file and extracting each word, there needs to be a check to see if we are using stop words, if yes then see if the word is within the set mentioned earlier otherwise we will add the word to the dictionary.


If we want to use stem words that we transform the word to use the root word and append any letters that are needed as well. Once that is done we add that to the dictionary.


The easy check for a dictionary is if the word is in the dictionary then we just increment the count; otherwise, we just insert it as a new word we saw with the value of 1. 


Finally, we sort the dicionary by the value so the most popular words are in the beginning of the dictionary.

##Step 3 Saving the results##


For the saving, we check if there is a file that exists, if not we create a new file otherwise we just create a file with the same file name with an appended number.

We are writing the top 25 or the number that the user inputs. We also write the list of stop words, if the user wants to use stop words, and the original text. 



##Libraries##

The libraries imported was:
io - for reading and writing files
os - to determine if a file exists on the operating system before creating a new file


##Set Up##

I built this application using Jupyter Notebook so the best installation steps are here: 
https://docs.anaconda.com/anaconda/install/index.html

I also used the individual package to run anaconda
https://www.anaconda.com/products/individual


Once anaconda is up and running you can open the file directly through the browser (automatically opens when running Anaconda). I use Chrome personally. You can access your OS's file storage and get to the Text Analysis file. Open it up and a new Jupyter Notebook tab opens. Next, for Mac users you can use the keyboard shortcut Shift + Enter to run a cell or you can click into a cell (Blue highlight to indicate you are in a cell) and use the navigation to run (Cell --> Run Cells). Make sure you run the cells in order. 



##Hours Spent##


I received this assessment Monday during the day. So I worked on this assignment for 2-3 hours per day since then so a total of 6-9 hours (varied because I don't have the exact time frame)
