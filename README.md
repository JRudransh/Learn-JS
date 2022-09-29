# Beginning with JavaScript
JavaScript came about as a joint effort between `Netscape Communications Corporation` and
`Sun Microsystems, Inc`. The news release of the new language came on `December 4, 1995`
back when `Netscape Navigator 2.0` was still in its beta version. `JavaScript version 1.0` became
available with the new browser. (Before its release as JavaScript, it was called `LiveScript`.)
JavaScript is an object-based, client-side scripting language that you can use to make Web
pages are more dynamic. To make sense of such a definition, let’s look at its important parts one by one.

## ECMAScript

The full form of `ECMA` is `European Computer Manufacturer's Association`. ECMAScript is a Standard for JavaScript. It is a trademark scripting language specification. JavaScript is a language based on ECMAScript. A standard for scripting languages like JavaScript is ECMAScript. JavaScript is considered as one of the most popular implementations of ECMAScript.

## Object Based
Object based means that JavaScript can use items called objects. However, the objects are not
class based (meaning no distinction is made between a class and an instance); instead, they are just general objects. You’ll learn how to work with JavaScript objects in Chapter 8. You don’t
need to understand them in any detail until you know a few other features of the language.

## Client Side
Client side means that JavaScript runs in the client (software) that the viewer is using, rather than on the Web server of the site serving the page. In this case, the client would be a Web browser. To make more sense of this, let’s take a look at how a server-side language works and how a client-side language works.


        <script>
            document.write("This writes text to the page");
        </script>

## Using the HTML Script Tags
Now that you have been introduced to JavaScript, you’re ready to start coding. Since JavaScript code is run from HTML documents, you need to know how to tell browsers to run your scripts. The most common way to set off a script is to use the HTML `<script> </script>` tags in your document. You can place your script tags in either the head or body section of an HTML document.

## Calling External Scripts

        <script type="text/javascript" src="main.js"></script>


## Writing a “Hello World” Script
Rather than write “Hello World,” you’ll use another line of text for this script: “Yes! I am
now a JavaScript coder!” This requires only a single line of code, using the document.write()
method, which writes a string of text to the document:

        <script type="text/javascript">
            document.write("Yes! I am now a JavaScript coder!");
        </script>

**********************
# Q & A
#### Q. Why is there a dot (.) in the document.write() command?
Document is one of JavaScript’s predefined objects, and write() is a predefined method of
the document object. The dot puts the object and the method together to make the function
work.

#### Q. How do I know when to add the script inside the head section and when to add it inside the body section?
The main situation in which to add a script to the body section of a document is when you
are writing something directly to the page. In many cases, most of the scripting can be
accomplished in the head section, since you can use functions to call the code in the body
section.
***************
## Inserting Comments on One Line
If you want to add commentary on a single line in your code, place a pair of forward slashes
before the text of the comment:

        // Your comment here
        document.write("This is cool!"); // writes out my opinion


## Adding Multiple-Line Comments

        /*
        My script will write some text into my HTML document!
        All of this text is ignored by the browser.
        */
        document.write("You can see me!");


# Understanding Variables
**A variable represents or holds a value. The actual value of a variable can be changed at any time.**

## Naming Variables
1. JavaScript variables are case sensitive
1. can contain alphabet numbers and _
1. can't start from number
1. avoid reserved keyword 
1. can't contain spaces
### reserved keywords
`abstract` `delete` `goto` `null` `throws` `as` `do` `if` `package` `transient` `boolean` `double` `implements` `private` `true` `break` `else` `import` `protected` `try` `byte` `enum` `in` `public` `typeof` `case` `export` `instanceof` `return` `use` `catch` `extends` `int` `short` `var` `char` `false` `interface` `static` `void` `class` `final` `is` `super` `volatile` `const` `finally` `long` `switch` `while` `continue` `float` `namespace` `synchronized` `with` `debugger` `for` `native` `this` `default` `function` `new` `throw`

## Understanding Data Types

### Number
Number variables are just that—numbers. JavaScript does not require numbers to be declared as integers, floating-point (decimal) numbers, or any other number type. Instead, any number is seen as just another number, whether it is 7, –2, 3.453, or anything else.

### String
String variables are variables that represent a string of text. The string may contain letters,
words, spaces, numbers, symbols, or most anything you like.

**Using Special Characters**

        Backslash (\)           \\
        Double quote (")        \"
        Single quote (')        \'
        Newline                 \n
        Tab                     \t


## Boolean

A Boolean variable is one with a value of true or false.

## Null

Null means that the variable has no value. It is not a space, nor is it a zero; it is simply nothing.

*********************

# Project

## Declare Variables

This project gives you the opportunity to practice declaring variables with various values. It also prints a short line of text on the page.

### Step by Step

1. Create an HTML page, leaving the space between the <body> and </body> tags open.
2. Between the <body> and </body> tags, add the <script> and </script>
3. Create a numeric variable named chipscost and give it the value 2.59
4. Create a Boolean variable named istrue and give it the value false
5. Create a variable named nada and give it the value null
6. Create a JavaScript statement to write to the Web page the string value that follows. Remember to escape quotation marks when necessary: `John said, “This project is fun!”`
7. The body section of the HTML document should look like this when you are finished:

        <body>
        <script type="text/javascript">
        var chipscost=2.59;
        var istrue=false;
        var nada=null;
        document.write("John said, \"This project is fun!\"");
        </script>
        </body>

8. Save the file as prj_1.html and view it in your Web browser.

## Using Variables in Scripts

### Making a Call to a Variable

        <script language="JavaScript">
            var mycar="Corvette";
            document.write(mycar);
        </script>

### Adding Variables to Text Strings

        <script type="text/javascript">
            var mycar="Corvette";
            document.write("I like driving my "+mycar);
        </script>

************

# Function

**What a Function Is**

A function is basically a little script within a larger script. Its purpose is to perform a single task or a series of tasks.

**Why Functions Are Useful**

Functions help organize the various parts of a script into the different tasks that must be
accomplished. By using one function for writing text and another for making a calculation, you
make it easier for yourself and others to see the purpose of each section of the script, and thus
debug it more easily.

## Declaring Functions

        function functionname() {
            // Code here
        }


### Naming Functions

As with variables, functions need to be named carefully to avoid problems with your scripts. The same basic rules that applied to variables apply to the naming of functions: case sensitivity, using allowed characters, avoiding reserved words, and giving functions memorable and meaningful names.

### Adding Parameters to Functions

Parameters are used to allow a function to import one or more values from somewhere outside
the function.

        function functionname(variable1,variable2)


### Adding Return Statements to Functions

A return statement is used to be sure that a function returns a specific value to the main script, to be used in the main script. You place the return statement as the last line of the function before the closing curly bracket and end it with a semicolon.


        function get_added_text() {
            var textpart1="This is ";
            var textpart2="fun!";
            var added_text=textpart1+textpart2;
            return added_text;
        }



### Calling Functions in Your Scripts

Now that you know how the function itself works, you need to learn how to call a function in your script. A call to a function in JavaScript is simply the function name along with the set of parentheses

        functionname();


### Calling a Function from Another Function

Calling a function within another function can be a useful way to organize the sequence in which your events will occur. Usually, the function is placed inside another function that has a larger task to finish.


        function update_alert(){
            window.alert("Welcome! This site is updated daily!");
        }

        function call_alert() {
            update_alert();
        }

        call_alert();


**Parameters Are Optional**

        function check_alert(pcheck,car) {
            window.alert("You make $"+pcheck+" and have a "+car);
        }
        check_alert();

        // You make $undefined and have a undefined

*************************

# Operators

## Understanding the Operator Types

### Mathematical 
These operators are most often used to perform mathematical calculations on two values. The mathematical operators will probably be the most familiar to you. They use symbols such as +, –, and *.
### Assignment
These operators are used to assign new values to variables. As you learned in Chapter 3, one of the assignment operators is the symbol =.
### Comparison
These operators are used to compare two values, two variables, or perhaps two longer statements. They use symbols such as > (for “is greater than”) and < (for “is less than”)

### Logical
These operators are used to compare two conditional statements (or to operate on one statement) to determine if the result is true and to proceed accordingly. They use symbols such as && (returns true if the statements on both sides of the operator are true) and || (returns true if a statement on either side of the operator is true).
### Bitwise
These are logical operators that work at the bit level (ones and zeros). They use symbols like << (for left-shifting bits) and >> (for right-shifting bits).

## Understanding Mathematical Operators

Operator         | Symbol | Function 
-----------------|--------|--------
Addition         |    +   | Adds two values
Subtraction      |    -   | Subtracts one value from another
Multiplication   |    *   | Multiplies two values
Exponentiation   |   **   | Raises the first operand to the power of the second operand
Division         |    /   | Divides one value by another
Modulus          |   %    | Divides one value by another and returns the remainder
Increment        |   ++   | Shortcut to add 1 to a single number
Decrement        |   --   | Shortcut to subtract 1 from a single number

## Understanding Assignment Operators
Operator| Example   | Same As
--------|-----------|--------
=       | x = y     | x = y
+=      | x += y    | x = x + y
-=      | x -= y    | x = x - y
*=      | x *= y    | x = x * y
/=      | x /= y 	| x = x / y
%=      | x %= y 	| x = x % y
**=     | x **= y 	| x = x ** y

## Understanding Comparison Operators

 Operator | 	Description
| ---------|-----------
| ==       | 	equal to
| ===      | 	equal value and equal type
| !=       | 	not equal
| !==      | 	not equal value or not equal type
| >        | 	greater than
| <        | 	less than
| >=       | 	greater than or equal to
| <=       | 	less than or equal to
| ?        | 	ternary operator

## Understanding Logical Operators

Operator    | 	Description
------------|-----------
| &&        | logical and
| \|\|      | logical or
| !         | logical not

## The Bitwise Operators

Operator        | Symbol
----------------|-----------
| AND           | &
| XOR           | ^
| OR            | \|
| NOT           | ~
| Left  Shift   | <<
| Right Shift   | >>
| Right Shift   | (Zero-Fill) >>>
