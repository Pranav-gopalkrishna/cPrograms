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

The difference is that in the first command, an executable file *a.out* is automatically created, while in the second command, you create the executable file *helloWorld*. To see the creation of these files with your own eyes, enter the command ```ls```.

Execute the program by typing ```helloWorld``` in the terminal.

If trying to execute the program leads to an error, it is because the program's location is not included in the PATH variable. PATH is an [environment variable](https://en.wikipedia.org/wiki/Environment_variable) that tells the shell, i.e. the terminal interface, which directories to search for executables in response to the commands issued by the user. For example, ```ls, mkdir, cd, rm, cp, mv...``` commands, which are stored in the *usr/bin* folder, are executable throughout the file system because the *usr/bin* folder is incuded in the PATH. 

To view the contents of the PATH variable, enter the following command.

```sh
echo $PATH
```

The input and output would be something like the following.

```sh
Pranavs-MacBook-Air:cPrograms pranav$ echo $PATH
/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin:
/Applications/VMware Fusion.app/Contents/Public:
/usr/local/share/dotnet:
~/.dotnet/tools:
/Library/Frameworks/Mono.framework/Versions/Current/Commands:
/Users/pranav/cPrograms/
```

If you want to add a directory to PATH, enter the following command.

```sh
export PATH=$PATH:/<yourWorkingDirectory>
```

## Additional information
To see all the environment variables in the file system, enter the command ```printenv```.


