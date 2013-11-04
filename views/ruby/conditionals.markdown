Conditionals

Goals
Use gets to get input from the user of your program.

Use a conditional statement to execute a branch of code only some of the time.
Step 1
Create a new file called conditionals_test.rb

Type this in the file conditionals_test.rb:
print "How many apples do you have? > "
apple_count = gets.to_i
puts "You have #{apple_count} apples."
Type this in the terminal:
ruby conditionals_test.rb
When prompted, type in a number of apples and press enter.

print is like puts but doesn't make a new line after printing.

gets, or get string, pauses your program and waits for the user to type something and hit the enter key. It then returns the value back to your program and continues execution. Since the user could have typed anything ('banana', '19.2', '<<!!@@') we use to_i to ensure what comes out is an integer. If the user didn't type a valid integer, to_i returns 0.

Step 2
Continuing on from the end of conditionals_test.rb...

Type this in the file conditionals_test.rb:
if apple_count > 5
  puts "Lots of apples!"
else
  puts 'Not many apples...'
end
Type this in the terminal:
ruby conditionals_test.rb
The if ... else ... end construct is a way of changing which lines of your program get executed depending on your data.

Try running the program with different values for apple_count to see each side of the conditional get executed.

Step 3
What goes after the if is any expression that returns a boolean, (the values true or false). Here's some more expressions that return true or false:

Type this in irb:
15 < 5
10 == 12
'foo' != 'bar'
Type this in irb:
'sandwich'.end_with?('h')
'sandwich'.end_with?('z')
[1,2,3].include?(2)
[1,2,3].include?(9)
Many methods return true or false as well. By convention, methods in Ruby that return booleans end with a question mark.

Step 4
You can nest a conditional in a loop, as well.

Create a new file called conditional_loops.rb

Type this in the file conditional_loops.rb:
fruits = ['apple', 'pear', 'apricot']
fruits.each do |fruit|
  if fruit.start_with?('a')
    puts "#{fruit} begins with the letter a."
  end
end
Type this in the terminal:
ruby conditional_loops.rb
Try changing this conditional so it only prints fruits with at least five letters in their name. Remember to change the string you're putsing as well!

Step 5
Create a new file called while_loop.rb

Type this in the file while_loop.rb:
total = 0
user_input = nil
while user_input != 'stop'
  print 'Enter a number to add to the total. > '
  user_input = gets.chomp
  total = total + user_input.to_i
end
puts "Your final total was #{total}!"
Type this in the terminal:
ruby while_loop.rb
A while loop continues repeating until a certain statement is false. Here, the program continually asks us for numbers until we say the string 'stop'.

It's easy for a while loop to get out of control! If your loop body doesn't do anything to make the while condition false, your loop will run forever.

Explanation
Without some kind of conditional, your program would do the same thing every time. Conditionals let you choose to do different things depending on what data you have in hand.

Now that you know conditionals, loops, arrays, hashes and strings, you can make some pretty complicated programs!

Next Step:
Go on to Functions