# Gulp-lang
Gulp is a deque-based, esoteric programming language created for use in code golfing. It has 128 commands, each one often having many functions at once. This tutorial will explain the basics of the language. All commands that are not explained here, will be in a chart soon to be in this repo.
# Syntax
Gulp's syntax is simple. It consists of one commamd followed by an argument. The only exceptions are commands which have to surround their arguments, and commands which have several arguments. Many "properties" in this language also affect the use of commands. e.g

    Properties{[Command][Argument(s)]}

This shows that the function of certain commands may be changed if they are modified with a property.

# I/O
Anything surrounded in single quotes is automatically pushed to the front of the deque, and printed. Take this Hello World Program as an example.

    'Hello, world!'

Furthermore, input is received from the user using the "j" command, and is automatically pushed to the front of the deque:

    j

This program will take user input and push it to the deque. The "k" command also pushes user input to the front of the deque and prints it.

# Variables
Variables are declared with the "o" command (notice how the o is lowercase. Gulp is case sensitive, so capital O has a different function). Following the "o" command is the variable identifier and the desired value of the variable.

    oi99

This program declares the variable "i" with integer value 99. When a variable is present in the program but not used as an argument it's value is printed:

    o

The above program will print the integer "99."

# Control Flow
Control flow in Gulp comes in the form of the if statement, "p". When p is used, it must be immediately followed by a condition, and the if body. Optionally, the if body may be followed by another p signifying an else body. We'll use the variable we defined in the last section as "99." 

    pi<100ip'100

This program checks if i is less than 100. If it is, then i is printed, otherwise, 100 is printed. There is a property that makes sure that any character used in the condition isn't confused with the same character in the if body. e.g

    pi<1000C:\FolderName\File.gu'i is less than 100'pC:\FolderName\File.gu i is less than 1000

This program is supposed to check if i is less than 100, not 1000. The extra 0 is a command that opens a file at a directory and writes something in it. In order to simplify this code, you have to seperate the two zeros with a semicolon. e.g

    pi<100;0C:\FolderName\File.gu'i is less than 100'pC:\FolderName\File.gu'i is less than 1000'

This would give the desired output, "i is less than 100". 
# Loops
There are no built in while or for loops in Gulp. However, there is a loop that takes an integer at the beginning of the loop, executes the given instructions in the loop, decrements the integer, and repeats this until the number has reached 0. e.g

    ow32(3w)

This program prints the integer 32, three times. Other types of loops can be implemented using the goto instructions that are present in Gulp. These commands are "v", which labels a section of code with a name that can be referenced later, and "w", which jumps to the specified label. 

Here is a "while" loop that prints integers 1 to 10.

    oc1vspc<11cc+ws

This  program declares variable c with value 1. Then, it labels the rest of code with the name "s." The program checks if c is less than 11. If it is, then c is printed and incremented, and the program jumps back to the beginning of the if statement.
