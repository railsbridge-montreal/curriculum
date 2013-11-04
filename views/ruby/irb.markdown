# irb

## Goals

- Understand the difference between irb and the command line
- Understand how and when to use irb
- Execute some simple ruby statements

### Step 1

Type this in the terminal:

`irb`

irb is the interactive ruby interpreter.

In irb, you can experiment with short pieces of code to figure out what they do.

### Step 2

Type this in irb:

```ruby
5 + 9
109 / 17
2 ** 8
5 > 6
```

What happened after each line? What do you think these statements do?

### Step 3
Lets take a closer look at the output of irb:

Type this in irb:

```ruby
1 + 2
```

Expected result:

```
1.9.3p125 :015 > 1 + 2
 => 3
1.9.3p125 :016 >
```

Here, `=> 3` is the return value of the statement `1 + 2`. Every statement in ruby has a return value: irb shows you that value after you type a complete statement and press enter.

### Step 4
Type this in irb:

```ruby
exit
```

exit is the guaranteed way to get out of irb. Depending on your operating system, Control-C or Control-D on an empty line may also work.

Practice going in and out of irb a couple of times. How can you tell when you're in or out of irb?

## Explanation

irb isn't a place to write code: it's a place to experiment and find out how certain language features work. When you write a full-fledged program, you'll save it into a text file on your computer.

## Next Step:
Go on to [Variables](variables)