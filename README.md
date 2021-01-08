# Veda's Notes


## Summary 

This repository contains all of the notes taken by Veda for the Lighthouse Labs Web Development Bootcamp.

## Day-1:
Linting and ESLInt setup:
Lint, or a linter, is a tool that analyzes source code to flag programming errors, bugs, stylistic errors, and suspicious constructs.
Time to install this awesome tool on our machine!

npm install -g eslint

Download the .eslintrc.json file into our /vagrant folder.
curl -o /vagrant/.eslintrc.json https://gist.githubusercontent.com/kvirani/6cdb9511522d4357839718a050e7dd3b/raw/.eslintrc.json

to run the eslint on any file.js
eslint file.js

# Command Line Args:What are Command Line Arguments?
Command line arguments are strings of text used to pass additional information to a program when an application is run through the command line interface (CLI) of an operating system. Command line arguments typically include information used to set configuration or property values for an application.
$ [runtime] [script_name] [argument-1 argument-2 argument-3 ... argument-n]
# Why Use Command Line Arguments?
The following are some of the major benefits of using command line arguments:

You can pass information to an application before it starts. This is particularly useful if you want to perform large number configuration settings.
Command line arguments are passed as strings to your program. String data types can easily be converted to other data types within an application, making the arguments very flexible.
You can pass unlimited number of arguments via the command line.
Command line arguments are used in conjunction with scripts and batch files, which is particularly useful for automated testing.
# Using process.argv
The simplest way of retrieving arguments in Node.js is via the process.argv array. This is a global object that you can use without importing any additional libraries to use it. You simply need to pass arguments to a Node.js application, just like we showed earlier, and these arguments can be accessed within the application via the process.argv array.

# console.assert
The console.assert() method writes an error message to the console if the assertion is false. If the assertion is true, nothing happens.




Day-4:Fun with callback functions


Functions do not need to be named, or even assigned to a variable. These are known as anonymous functions.
Anonymous functions are often declared while being passed in as callbacks to other functions. Why? Because the receiving function that takes in the anonymous function will give that parameter a name anyway.

Higher-Order functions are any functions which operate on other functions.
This includes, but is not limited to, functions which take in functions (callbacks) as arguments.

This means that built-in functions such as forEach, filter, and others can be called "Higher-Order Functions".
