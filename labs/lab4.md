
Navigate to your untrimmed_fastq directory in one line

### Exercise
Find the line number in your history for the command that listed all the .sh files in /usr/bin. Rerun that command.

### EXERCISE
Print out the contents of the ~/shell_data/untrimmed_fastq/SRR097977.fastq file. What is the last line of the file?
From your home directory, and without changing directories, use one short command to print the contents of all of the files in the ~/shell_data/untrimmed_fastq directory.








### File Permissions
The first part of the output for the `-l` flag gives you information about the file's current permissions. There are ten slots in the
permissions list. The first character in this list is related to file type, not permissions, so we'll ignore it for now. The next three
characters relate to the permissions that the file owner has, the next three relate to the permissions for group members, and the final
three characters specify what other users outside of your group can do with the file. We're going to concentrate on the three positions
that deal with your permissions (as the file owner).

![](fig/rwx_figure.svg){alt='Permissions breakdown'}

Here the three positions that relate to the file owner are `rw-`. The `r` means that you have permission to read the file, the `w`
indicates that you have permission to write to (i.e. make changes to) the file, and the third position is a `-`, indicating that you
don't have permission to carry out the ability encoded by that space (this is the space where `x` or executable ability is stored, we'll
talk more about this later.


## Exercises

`echo` is a built-in shell command that writes its arguments, like a line of text to standard output.
The `echo` command can also be used with pattern matching characters, such as wildcard characters.
Here we will use the `echo` command to see how the wildcard character is interpreted by the shell.

```bash
$ echo *.fastq
```

```output
SRR097977.fastq SRR098026.fastq
```

The `*` is expanded to include any file that ends with `.fastq`. We can see that the output of
`echo *.fastq` is the same as that of `ls *.fastq`.

What would the output look like if the wildcard could *not* be matched? Compare the outputs of
`echo *.missing` and `ls *.missing`.



NAVIGATING PRACTICE
Navigate to your home directory. From there, list the contents of the untrimmed_fastq directory.

FINDING HIDDEN DIRECTORIES
First navigate to the shell_data directory. There is a hidden directory within this directory. Explore the options for ls to find out how to see hidden directories. List the contents of the directory and identify the name of the text file in that directory.

Hint: hidden files and folders in Unix start with ., for example .my_hidden_directory