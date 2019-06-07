# Learning R: Comparing R to Java


*Maria Matlick*
*Published June 6th, 2019*

For many students at the University of Washington, they learn the coding language "Java" first. Introduced in the
Computer Science and Engineering 14x series, students can become professionally proficient in Java in two short
quarters. These classes are prerequisites for many majors-including Math, Computer Science, and Informatics. For
many Informatics students, they then learn R through the Info 201 class, which is a required pre-requisite to apply
for the major. Many experienced coders say that after learning one language, in this case **Java**, learning a second
is much easier, so in this case **R**. I am going to share my experience and some tips and tricks when learning R with
a background in Java at the University of Washington. There are pros and cons to both!

## First Things First: The Basics
### Parenthesis
#### Java
In the 14x series, students learn and use Java using the compiler called *JGrasp*. Unbeknownst to first time coders,
this compiler is looked down upon by more experienced coders, considered clunky and not that useful when there are better
options out there. A basic trick first time coders learn in CSE 142, is to always type the matching parenthesis in order
to not forget them later.  

*For Example:* <br />
Java coders diligently type <br />
`System.out.print(` <br />
Then, immediately close the parenthesis, <br />
`System.out.print()`<br />
<br />
And go back to type in between the parenthesis.
#### R
However, when students new to R begin typing in compiler Rstudio, they
experience something just about magical. No matter what function they type, and what kind of parenthesis (whether
basic parenthesis, square brackets, curly braces, **even quotation marks**, etc), Rstudio not only automatically types
the closing parenthesis, but leaves the user's cursor in between them. <br />
*For example:* <br />
R coders can type <br />
`print()` <br />
With Rstudio making parenthesis absurdly easy. This is extremely helpful in eliminating parenthesis related compiler errors. Another
crazy trick with parenthesis and quotation marks is that if a user typed, for example, <br />
`print(Hello World)`, and forgot the quotation marks, they can highlight "Hello World", type a single quotation mark, and suddenly they see <br />
`print("Hello World")` <br />
Incredible! <br />
<br />

### Printing
#### Java
As you may have seen above, printing text is slightly different in R and Java. In Java, there are **two main ways** to print
and output text. Users in Java must remember to type two long sentences with correct capitalization in order to print text.  

*For Example:* <br />
Java users have to complete typing <br />
`System.out.print("Hello World")` <br />
While remembering to close the parenthesis, move their cursor back between them, and manually type both quotation marks in order
to print something, and there is *no autocomplete in JGrasp*. If they would like to print text with a new line afterwards,
the coder must type, <br />
`System.out.println("Hello World")` <br />
again, with correct capitalization and coding grammar. Luckily for students in the 14x series, they are allowed to abbreviate
*two things* on their midterm and final exams.
`System.out.print("Hello World")` can become `S.o.p("Hello World")` <br />
and <br />
`System.out.println("Hello World")` can become `S.o.pln("Hello World")` <br />
Thank the coding gods! <br />
<br />
#### R
On the contrary, in R, users have many different options to print and output text. Maybe too many? Functions we will look at today include
`print()`and `cat()`. Let's start with the basics, and we won't go *too* in depth in the complexities of these functions.
 When you want to print something, anything, whether it be a character string or include numbers, coders use <br />
 `print()`. The "p" **must be lowercase**. Here are some examples: <br />
 `print("Hello World")` <br />
 `print("He110 W0rld 1234")` <br />
 `print("13579")` <br />
In order to make a new line, users must include `\n`. For example, <br />
`print("Hello World \n")`. <br />
It is also important to note that in R, quotation marks (") and the symbol mainly used for apostrophes, ('), are interchangeable **throughout all R code**. This means that
coders can type <br />
`print("Hello Word")` or `print('Hello World')` and output the same text. This outputted text will have the quotation marks surrounding it: <br />
**Coder types:** `print("Hello World")` <br />
**Compiler outputs:** "Hello World" <br />
<br />
Moving on to `cat()`. "cat" comes from *concatenate*, a word Java coders are familiar with. One of my favorite things to do with `cat()` is to take
multiple words, and put them together using this function. For example, if for whatever reason a user wanted to type their words separately, they can. <br />
`cat("Hello", "World")` <br />
This is also really helpful when using variables, which we will get into later. But for now, since all Java users understand variables, we will
use them as examples anyways. Let's say I make two variables, <br />
`x <- "Hello"` and <br />
`y <- "World"` <br />
I can them concatenate them into a single string, by saying <br />
 **Coder types:** `cat(x, y)` <br />
 **Compiler Outputs:** Hello World <br />
 Notice there are no quotation marks around this text! `cat()` can also convert files into text that shows up in the compiler output. Now, in all of
 my examples using `cat()`, I have separated each word or variable with a comma. If you want to change how to separate them, you can add in `sep =`
 and then input whatever character you want to sparate them by. For example: <br />
 `cat("Hello" "World", sep = " ")` <br />
 In this case, what separates the separate words is a space, not a comma. <br />
 <br />
### Variables
#### Java
 In Java and R, defining variables is integral to the coding process. In Java, this is much more specific than it is in R. To assign a variable in Java,
 one must define what type the variable is. Meaning, if the variable is going to be an integer (meaning a whole number, not a decimal), the coder types <br />
 `int number = 2` <br />
 If they want it to be a character string, the coder would type: <br />
 `String string = "Hello World"`.<br />
  Or if they wanted a double (a number with a decimal), they would type <br />
  `double decimal = 2.345` <br />
  When defining a variable, the coder just uses the `=` to set what the variable is equal to. In Java, words are also using camel casing, whichLooksLikeThis. That way, if a variable needs multiple words to define it, it would look like this <br />
  `thisIsComplicated = "This variable needed a longer definition"` <br />
 <br />
 #### R
 In R, defining variables is a lot more ambiguous. And, you don't use the `=` sign, you use `<-`. This sign can be typed quickly
 by using the shortcut alt + -. Variable examples include: <br />
 `number <- 3` <br />
 `decimal <- 3.456` <br />
 `string <- "Hello World"` <br />
 Instead of camel casing, R separates words using `_`. For example, <br />
 `this_is_complicated <- "This variable needed a longer definition"` <br />
 <br />

 ## Conclusion
There you go, a basic introduction to some basic differences in R and Java, and some tricks to understand what to do in each language.
