# Lab3 - 2/6/26

## Before lab begins
1. Open up vscode
2. Control + shift + 'p' to open command prompt (command + shift + p on apple)
3. Start typing 'Connect to...' and the 'Connect current window to host' menu item will pop up. Select it
4. If asked, connect to 'ron.sr.edu host'
5. Enter your RON username if prompted
6. Enter your RON password when prompted
7. Go to 'File --> Open folder'
8. Select your 'gen711-811' directory
9. If you haven't done so already, save your workspace to this directory (File --> save directory as --> enter)
10. Take your notes in 'Markdown' format. See the readme.txt for taking notes for this lab below. 

# Part 1 (lab 3)
### Questions:
- What is a command shell and why would I use one?
- How can I move around on my computer?
- How can I see what files and directories I have?
- How can I specify the location of a file or directory on my computer?

### Objectives:
- Describe key reasons for learning shell.
- Navigate your file system using the command line.
- Access and read help files for bash programs and use help files to identify useful command options.
- Demonstrate the use of tab completion, and explain its advantages.

## The key points here are:
- The shell gives you the ability to work more efficiently by using keyboard commands rather than a GUI.
- Useful commands for navigating your file system include: ls, pwd, and cd.
- Most commands take options (flags) which begin with a -.
- Tab completion can reduce errors from mistyping and make work more efficient in the shell.

# Navigating Files and Directories
- How can I perform operations on files outside of my working directory?
- What are some navigational shortcuts I can use to make my work more efficient?

# Part 2 (lab 3)
## Objectives:
- Use a single command to navigate multiple steps in your directory structure, including moving backwards (one level up).
- Perform operations on files in directories outside your working directory.
- Work with hidden directories and hidden files.
- Interconvert between absolute and relative paths.
- Employ navigational shortcuts to move around your file system.

## More navigation
- We got an idea for moving around using cd and the name of the folder to move into. 
- But how to we go back out? We dont see the folder we are in.
- We have a special command to tell the computer to move us back or up one directory level.

### Your Notes Here: 
Seperate notes by an empty line, or they'll get pasted together

- Using a dash is helpful for lists
1. And numbers for lists

The pound sign is used for 'sections'. A single pound (or hashtag) in front of a word makes it appear bigger/bold to show a new section. See below

# My Notes:

To change directories, use 'cd' and then hit tab two times to see directories in my current directory

1. pwd = print working directory

directories can contain files or folders

2. ls = list
ls ' = bumps to new line, waiting for other end of quote '
use ctrl+c to exit = used to cancel

3. cd shell_data
4. ls
ls -F = adds slashes st end of directories
man ls = manual, give operator manual for ls
q exits to command line
ls -lrth = directories and owners, creation date, permissions listed

5. cd untrimmed_fastq/
start with cd u then tab to autofill
in eh1223@ron untrimmed_fastq

6. ls
head S tab 7 or 8 tab.fastq
lists genome data in form of fastQ

to get out
1. cd ../
in eh1223@ron shell_data, one step out
../../ is two steps out
etc
cd ~ 
~ = shorthand for home directory
then cd DIRECTORY

rm = remove, equivalent to delete
anything not pushed to git will be deleted
$VARIABLE = takes to variable site
echo shows paths within VARIABLE

history = shows entire command history
bottom most recent, top oldest

grep = basically ctrlF, searches lines for specific things

^ = beginning of line
ex. grep '^@'
shows results with @ at beginning of line

head = shows first few lines of a file

ls *FILE
* = wildcard, anything works
only listed files after *

ws = word count
gives line #, word #, character #
ls /bin/LETTER* | wc -l
gives word count for files in /bin that start with LETTER
-l = lines

less = allows scrolling through files


### Complete the questions below when intrstructed. Push the changes to this document to recive credit for attending the lab

#### 1. What are 3 ways to change directories to your home directory from the  untrimmed_fastq directory?
1.
2.
3.

#### 3b. How many programs in /bin 
2. Do each of the following tasks from your current directory using a single ls command for each:
    - List all of the files in /bin that start with the letter ‘c’.
    ls safdasfsla
    - List all of the files in /bin that contain the letter ‘a’.
    - List all of the files in /bin that end with the letter ‘o’.
    - Bonus: List all of the files in /bin that contain the letter ‘a’ or the letter ‘c’.

#### Answers here
Start with the letter c ____
Start with the letter a ____
Start with the letter o ____
Contain the letter ‘a’ or the letter ‘c’ ____

#### What command/commands would you use to find the line number in your history for the command that listed all the '.fastq' files using the absolute path. Paste your answer below.

ls gdsfgsd 
