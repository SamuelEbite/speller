# speller
This is my solution to the speller problem set in the CS50 Introduction to Computer Science course. The program implements a spell checker that reads in a text file and identifies any misspelled words by checking them against a dictionary file.

Usage

To run the program, you will need to have the following software installed on your computer:

A C compiler such as GCC or Clang
The CS50 library, which you can download from https://github.com/cs50/libcs50
Here are the steps to run the program:

Download the speller directory from the CS50 problem set repository
Compile the program using the following command:
ruby
Copy code
$ gcc -o speller speller.c dictionary.c hashtable.c -lcs50 -lm
Run the program with the following command, specifying the name of the text file you want to check:
shell
Copy code
$ ./speller text.txt
The program will output any misspelled words and the amount of time it took to load the dictionary and check the spelling.
Files

speller.c: The main program that reads in the dictionary file, loads it into a hash table, reads in a text file, checks the spelling of each word, and outputs any misspelled words.
dictionary.c: The implementation of the dictionary data structure, including functions for loading and unloading the dictionary, and for checking the spelling of a word.
hashtable.c: The implementation of the hash table data structure, including functions for inserting, searching, and deleting key-value pairs.
Implementation Details

The program uses a hash table data structure to efficiently store the words in the dictionary and perform fast lookups when checking the spelling of a text file. It also implements a hash function to generate unique indices into the hash table based on the string value of the word being stored.

The program uses memory allocation functions like malloc() and free() to dynamically allocate and deallocate memory for the hash table and the dictionary. It also includes error checking to handle any memory allocation failures.

Credits

This program was created as part of the CS50 Introduction to Computer Science course offered by Harvard University. The problem set was designed by the CS50 staff. The code implementation is my own work.
