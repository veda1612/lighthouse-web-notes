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




## Day-4:Fun with callback functions


Functions do not need to be named, or even assigned to a variable. These are known as anonymous functions.
Anonymous functions are often declared while being passed in as callbacks to other functions. Why? Because the receiving function that takes in the anonymous function will give that parameter a name anyway.

Higher-Order functions are any functions which operate on other functions.
This includes, but is not limited to, functions which take in functions (callbacks) as arguments.

This means that built-in functions such as forEach, filter, and others can be called "Higher-Order Functions".
# Arrow Functions
Arrow Function syntax can vary based on how simple the function is
Arrow functions don't get assigned a value for this (in the way that traditional function expressions do).
This "limitation" is in fact intentional, and can be used as an advantage in certain situations - situations where it is beneficial to inherit the value of this from its lexical scope. Such as the this.firstName being read in the sayHello method.


## Day-5:Recursion Intro

Recursion is an alternative to traditional looping that allows you to do the same thing, just in a slightly different way. Recursion isn't necessarily a better way of doing this, it's just a different way of doing this.
A recursive function will call itself to execute code over and over again, kind of like a loop. And like a loop, it has to stop calling itself at some point so that it doesn't keep repeating forever.
The recursive case is when the function will continue to call itself. Every time the function calls itself, the input gets closer and closer to the base case. The base case is when the function no longer calls itself. In a properly designed recursive function, with each recursive call, the input must gradually resolve toward the base case.

Recursion is a tool you can use as an alternative to traditional iteration using for and while loops.
Every recursive function must have a base case and a recursive case.
Each recursive call should break down the current problem into a smaller, simpler one.
The recursive calls must eventually reach the smallest version of the problem, the base case.
The base case is when the problem can be solved without further recursion.


## Day-6

# What are Unit Testing, Integration Testing and Functional Testing?
# What is unit testing:
https://codeutopia.net/blog/2015/04/11/what-are-unit-testing-integration-testing-and-functional-testing/
The core idea with unit testing is to test a function’s behavior when giving it a certain set of inputs. You call a function with certain parameters, and check you got the correct result.
Unit testing is the practice of testing small pieces of code, typically individual functions, alone and isolated. If your test uses some external resource, like the network or a database, it’s not a unit test.

Popular tools for unit testing include Mocha, Jasmine and Tape.
# Integration testing:
As the name suggests, in integration testing the idea is to test how parts of the system work together – the integration of the parts. Integration tests are similar to unit tests, but there’s one big difference: while unit tests are isolated from other components, integration tests are not. For example, a unit test for database access code would not talk to a real database, but an integration test would.
You should have fewer integration tests than unit tests. You should mainly use them if you need to test two separate systems together, or if a piece of code is too complex to unit test. But in the latter case, I would recommend fixing the code so it’s easy to unit test instead.

Integration tests can usually be written with the same tools as unit tests.

# Functional testing:
Functional testing is also sometimes called E2E testing, or browser testing. They all refer to the same thing.
Functional testing is defined as the testing of complete functionality of some application. In practice with web apps, this means using some tool to automate a browser, which is then used to click around on the pages to test the application.

The most common tool used for functional testing is Selenium. Running Selenium is usually done with Selenium WebDriver, or Protractor. Sometimes PhantomJS and CasperJS can be used as well, especially if you don’t need to test in real browsers.

https://codeutopia.net/blog/2015/03/01/unit-testing-tdd-and-bdd/

# Happy path testing:





# BDD Frameworks:
BDD or Behavior Driven Development is a process that emerged from test-driven development in 2006.
BDD encourages you to specify the behavior of your app in terms of user stories which are broken down into scenarios that can be built and tested.
Mocha testing framework and the Chai assertion library. These are very popular packages for testing javascript and are very easy to get started with.

Mocha gives us the describe and it functions. Each it is a test, and each test should have at least one assertion.
Chai is an assertion library. It gives us assertion functions so that we no longer have to use our assertEqual and other assertion functions that we implemented previously. Chai assertion functions are deliberately designed to play nice with testing frameworks like Mocha.



## Intro to net:
Net (net) is a module that is built into Node. It allows our Node apps to use TCP.




