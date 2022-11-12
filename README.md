 C - BUILD YOUR OWN SHELL
## Introduction: :ledger:
* One of the core tenets of the ALX SE program is the belef in ding hard things and now, they have presented us with another hard thing
* The mission of this current task is to build a shell that will work as good as any bash shell or even better
* As usual, there are restraints and constraints on the number and type of functions we're allowed to use but the fact that we're working in teams of two means that we have more info and resources to use

## Helper Files: :raised_hands:
Every file is a helper file though as ALX didn't provide us with the usual _putchar function

## Header Files: :scroll:
* [shell.h](./shell.h)
It contains all the header files we should have been constantly declaring to usse functions and syscalls like the write and read_

## Contents
* ### Files which are sourcefiles for the codes :page_facing_up:
|**FILES**|**FUNCTIONS**|**ACTIONS**|
|:---|:---:|:---|
|[append.c](./append.c)|_int appendStr(char ***arr, size_t *size, char *str, int index)_|Appends a string to an array of strings_|
||int appendChar(char **string, size_t *size, char chr, int index)|Appends a  character to a string_|
|[find.c](./find.c)|char *findenv(char *env[], const char *name)|Returns the value of a n environmental variable|
||struct dirent *findfile(DIR *dir, const char *filename)|searches through the directory for a a file|
||char *joinpath(const char *base, const char *child)|Joins two paths together using "/"|
||char *findcmd(const char *command, const char *PATH)|searches throuh the $PATH variable to find a command|
|[line.c](./line.c)|char **tokenizeLine(char *line)|Split a line into separate words|
|[qoute.c](./quote.c)|int findquote(char *str, char quote)|Finds a string in quotes within a string(unescaped quote)|
||int parsequote(char *string, int *index, char **buffer, size_t *buf_size, int *buf_index)|Groups characters in quotes as a single word during tokenization|
|[run.c](./run.c)|int execute(const char *program, char *args[])|Executes a programin a child process|

* ### _Files with a program as a target_ :page_with_curl:
|**FILE**|**PROGRAM FUNCTION**|
|:---|:---:|
|[main.c](./main.c)|It is the entry point for the shell|

## See Also
 <details>
  <summary>Please click this arrow for compilation instructions</summary>

  * Use **_gcc *.c -o hsh_** to compile
  * THen run **./hsh**
  * Ignore any .swo, .swp and any other file that is not an executable, C or header file
  * This shell is experimental meaning that you use at your own risk
</details>

## AUTHORS
**Samuel Nathaniel** alias **BlissNathan** :stuck_out_tongue_winking_eye::v:
* To view my github, click [here](https://github.com/BlissNathan1305) 

**Mongikazi Mzomba** alias **Santee12** :sunglasses::ok_hand:
* To view my github, click [here](https://github.com/Mzombam/Mzombam))
