Strings

Goals
Understand when to use strings
Learn how to combine strings
Learn about string interpolation
Step 1
Type this in irb:
'a string in single quotes'
"a string in double quotes"
A string is a series of characters. Strings can be created using either single or double quotes.

These strings weren't saved into a variable. What happens to data not saved into a variable?

What happens if you start a string with one kind of quote and end with another? How can you fix it?

Step 2
Type this in irb:
'Hello, ' + 'Jane'
'apples' * 3
Strings can be added to each other or multipled by numbers. What does this do?

Step 3
Type this in irb:
name = 'Jane'
"Hello #{name}"
(the {} characters are generally called curly braces)

This is called string interpolation. String interpolation lets you embed a ruby statement in another string. It only works with double quotes: what happens when you try the same thing with single quotes?

Type this in irb:
"Two plus two is #{2 + 2}"
The code in the curly braces can be any valid ruby statement. Try putting various things in the curly brackets to see what works and what doesn't.

Step 4
Type this in irb:
'I have many characters'.length
The thing after the dot is called a method. Methods are things you can do to a given object: more on Objects later, just recognize here that the Object is a String.

Here's some more methods for you to try:

Type this in irb:
'forwards'.reverse
'jane smith'.upcase
'a plain old sentence'.delete('aeiou')
'some string'.methods
There's a method that's simply called methods -- it tells you all the methods you can use on a given object.

Explanation
Strings are a key way to present information in your programs. Since a human will probably be reading the output of your program eventually, and humans speak words rather than numbers, you will often want to use strings.

A not at all complete summary of methods on String:

length  how long is this string (characters)
reverse return same string, reversed
upcase  return same string, IN UPPER CASE
delete([another string])  delete all characters in the second string from the first
methods get the names of all methods you can perform on string
Further Reading
Ruby's documentation for String
Next Step:
Go on to Arrays