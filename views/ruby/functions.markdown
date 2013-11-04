# Functions

## Goals

- Create a function
- Call a function

### Step 1

Create a new file called area.rb

Type this in the file area.rb:

```ruby
def circle_area(radius)
  Math::PI * (radius ** 2)
end

print "What is the radius of your circle? > "
radius = gets.to_i

puts "Your circle has an area of #{circle_area(radius)}"
```

Type this in the terminal:

```bash
ruby area.rb
```

When prompted, type in a radius for your circle.

## Explanation
As your programs get more and more complicated, you'll want to group code into functions that can be called over and over again.

A function begins with def, followed by the function name. Next comes any variables it takes, followed by the actual body of the function. Lastly, function definitions are finished with the end keyword.

Pedantic Programmers might want to tell you that Ruby doesn't technically have functions, and everything in ruby is really a method. It is appropriate to slap these people.

Next Step:
Go on to [Objects](objects)
