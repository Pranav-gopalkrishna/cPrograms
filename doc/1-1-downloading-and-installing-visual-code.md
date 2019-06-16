[<< Go to table of contents](../readme.md)
# 1.1 Downlaoding and installing Visual Code

Visual studio code can be installed from [here](https://code.visualstudio.com/Download)

After instaling this, [C/C++ extention](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools) must be installed.

Next, XCode command line tools need to be installed. To do this, go to terminal and run the command below.

```sh
 xcode-select --install
 ```
 
### Common errors
 
 Without these tools, you will get the following error while compiling programs using the command-line code.
 
 ```sh
 xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at:
 /Library/Developer/CommandLineTools/usr/bin/xcrun
```
[Go to next chapter (1.2 Writing and compiling helloWorld.c) >>](1-2-writing-and-compiling-helloWorld.md)
