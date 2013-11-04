Running Programs From A File

Goals
Write a ruby program into a file
Execute a ruby program stored in a file
Step 1
In your text editor, create a file called my_program.rb

Type this in the file my_program.rb:
puts 'This code is in a file!'
some_variable = 19
puts "I stored a variable with the value 19!"
Step 2
Type this in the terminal:
ruby my_program.rb
You should have seen the output of your program: 'This code is in a file...' etc. If you didn't, you might not be in the directory where you created the file. See if it shows up in ls.

Explanation
Actual ruby programs aren't written in irb, they're written in files. As your program becomes larger and larger, it may span many files!

Next Step:
Go on to Conditionals