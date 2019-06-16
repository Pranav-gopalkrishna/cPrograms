[<< Go to table of contents](/doc/cPrograms/readme.md)

[<< Go to previous chapter (1.1 Downloading and installing Visual Code)](/doc/1-1-downloading-and-installing-visual-code.md)

# 1.2 Writing and compiling helloWorld.c

Here is the C program outputting the string "Hello world".

```c
#include <stdio.h>
int main()
{
    printf("Hello world \n");
    return 0;
}
```

The Unix command for compiling is gcc. GCC is a compilier from the [GNU project](https://www.gnu.org/), and it stands for GNU Compilier Collections. To compile the C program in command-line, enter the following command. 

```sh
gcc helloWorld.c
```

The full syntax is as follows.

```sh
gcc helloWorld.c -o helloWorld
```

The difference is that in the first command, an executable file ```a.out``` is automatically created, while in the second command, you create the executable file ```helloWorld```. To see the creation of these files with your own eyes, enter the command ```ls```.
