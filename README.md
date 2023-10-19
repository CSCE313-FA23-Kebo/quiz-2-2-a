# Quiz 2.2.a: file stats

Write a C program that takes a directory name as input and gives information about the named files in the directory.

## Print the files information
For every file in the directory, print the following information.

- File name
- inode number
- number of links
- User ID of owner
- Group ID of owner
- Size in bytes
- Last access
- Last modification
- Last status change
- Number of disk blocks allocated
- Access mode in octal
- Access mode flags

## Important notes:
1. Refer to the sample output [sample_output.txt](sample_output.txt) as an example of file stats for the directory [games](games).
1. Usage: `./filestats directory_name`
1. **Linux timestamps** hold a number rather than a date and time. When Linux needs to display a timestamp, it translates this number into a date and time. You can use the call `ctime(t)` to convert the calendar time `t` into a null-terminated string of the form `Wed Jun 30 21:49:08 1993\n`.
1. Your program will be manually tested for correctness with additional test cases including different file types.
1. Your program should compile with no errors and warnings.
