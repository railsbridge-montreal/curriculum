# Loops

## Goals

- Use loops to do operations for every element in an array.
- Use `puts` to print strings to the screen.
- Learn the two different syntaxes for creating blocks in Ruby.

## Step 1

Type this in irb:

```ruby
puts 'Hello World'
```

`puts` (*put* string) is a way of printing information to the user of your program.

Take some time to contemplate the output of `puts` in irb:

Expected result:

```bash
1.9.3p125 :006 > puts 'Hello World'
Hello World
 => nil
1.9.3p125 :007 >
```

The method `puts` always has the *return value* of `nil`, which is what we see after the `=>` in the output. Printing 'Hello World' to the screen is just a side-effect.

###Step 2

Type this in irb:

```ruby
fruits = ['peach', 'plum', 'pear']
fruits.each { |fruit| puts fruit }
```

The straight up-and-down `|` is called the 'pipe character', and is typically the shifted version of the `\` (backslash) on your keyboard.

Loops are a way of doing something here multiple times. In this loop, we printed each fruit to the screen in order.

###Step 3

Type this in irb:

```ruby
numbers = [109, 10, 1001]
numbers.each { |n| puts n * 2 }
```

The curly braces here define a *block*, and whatever's in the pipes is a *block variable*.

`each` takes the first element in the array and sends it to the block, which temporarily stores it in the *block variable* and then runs the code after the pipes. It then goes back and does this again for each of the remaining items in the array.

Type this in irb:

```ruby
ducks = ['huey', 'dewey', 'louie']
ducks.each { |duck| puts "#{duck} quacks!" }
ducks.each { |zombie| puts "#{zombie} quacks!" }
```

It doesn't matter what you call your block variable: the previous two statements are exactly equivalent to Ruby. But you should try to name your variables something useful so the code makes sense to you later!

### Step 4

Type this in irb:

```ruby
total = 256 ** 3
colors = ['red', 'blue', 'green']
colors.each do |color|
  puts "#{total} colors of paint on the wall..."
  puts "Take #{color} down, pass it around..."
  total = total - 1
  puts "#{total} colors of paint on the wall!"
end
```

The `**` operator means 'to the power of', as in '256 to the third power'

There's more than one way to make a block in ruby. The `do ... end` syntax is typically used when a block needs to span multiple lines, while the `{ ... }` syntax is for a single line block.

## Explanation
As you build complex programs, you'll want to do something to many pieces of data without typing it all out. Loops help solve this problem.

Next Step:
Go on to [Running Programs From A File](running_programs_from_a_file)
