# Gulp-lang
Gulp is an esoteric, deque based, golfing programming language made to win many CG challenges. It has 128 commands, each one often having many functions at once. This tutorial will run you through the basics in order to start programming right away. All commamds that are not explained here, will be in a chart soon to be in this repo.
# Syntax
The syntax of Gulp is very simple. It consists of one commamd folllwed by a parameter. The only exceptions are commamds which have to surround their parameters, and commands which have several parameters. Many properties in this language also affect the use of commands. 
# Printing
Printing is simple in this language. Anything surroumded in single quotes is automatically pushed to the front of the deque, and printed. Take this Hello World Program as an example.

'Hello, world!'

As  mentioned before, Gulp has properties that make golfing easier. One of these properties is auto quotation. When a string literal without the closing single quote is entered, then its still valid. The interpreter treats it the same way as a complete steing literal. e.g

'Hello, world!

This is still valid. There are still many commamds, however, that deal with printing as part of their functions. 
# Variables
Variablez are an important part of golfing. Which is why variables are easy to understand. Variables are declared with the    "o" command (notice how the o is lowercase. Gulp is case sensitive, so capital O has a different function). Fooloowing the o command is a variable name, which can only be 1 byte in lenth, and the value of the variable. e.f

oi99

This program declares the variable i with value 99. When a variable is used by itself, and it is not a parameter of a command, it's value is printed. e.g

o

Will print the integer 99.
# Control Flow
Control flow in Gulp comes in the form of the if statement, "p". When p is used, it must be immediately followed by a condition, and the if body. Optionally, the if body may be followed by another p signifying an else body. We'll use our variable "i" defined in the last section. 

pi<100ip'100

This program checks if i is less than 100. If it is, then i is printed, otherwise, 100 is printed. There is a property that makes sure that any character used in the condition isn't confused with the same character in the if body. e.g

pi<1000C:\FolderName\File.gu'i is less than 100'pC:\FolderName\File.gu i is less than 1000

This program actually checks if i is less than 100, not 1000. The extra 0 is a command that opens a file at a directory and writes something in it. In order to simplify this code, you have to seperate the two zeros with a p. e.g

pi<100p0C:\FolderName\File.gu'i is less than 100'pC:\FolderName\File.gu i is less than 1000

This would give the desired output, "i is less than 100".
