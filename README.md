## Division-and-Modulo-Calculator-GNU-Bash-v4

### Installation Instructions

    sudo mv <file> /usr/local/bin

    sudo chown $USER: /usr/local/bin/math

    chmod ug+rwx /usr/local/bin/math

Now you can access the file with the "math" command

You can type `math -h` for details on how to use the script with examples, but here are the basics:
-   It takes two numbers as arguments, the dividend and the divisor
-   The `-d` flag is for division and the `-m` flag is for modulo
-   The flags `-f` and `-c` represent floor and ceiling respectively
-   Default is `-mf` for paired sign integers and `-mc` for non-paired sign integers
-   The `-r` flag ensures the sign of the output is always positive


It's worth noting that if you use the truncated method for modulo, this script is by no means faster or even close to being equally fast to just using the "%" symbol, especially if lots of iterations are needed and speed is imperative. However, if specifically the floor of a ceiling is needed for a division or modulo operation, then this provides a simple interface to perform that function. Alternatively, the specific expression can be pulled from the file and used manually. Do what you want, it's open source after all.
