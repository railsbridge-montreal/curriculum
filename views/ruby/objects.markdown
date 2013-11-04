Objects

Goals
Define a new object
Create an instance of your object
Call methods on your object
Step 1
Create a new file called circle.rb

Type this in the file circle.rb:
class Circle
  def initialize(radius)
    @radius = radius
  end

  def area
    Math::PI * (@radius ** 2)
  end

  def perimeter
    2 * Math::PI * @radius
  end
end

print "What is the radius of your circle? > "
radius = gets.to_i

a_circle = Circle.new(radius)
puts "Your circle has an area of #{a_circle.area}"
puts "Your circle has a perimeter of #{a_circle.perimeter}"
Type this in the terminal:
ruby circle.rb
When prompted, type in a radius for your circle.

Explanation
Functions by themselves aren't always enough to keep your program organized. Object-oriented programming was developed to keep related data (attributes) and functions that work on that data (methods) together.

In Ruby, a new object is defined with the class keyword, followed by the name of your object (typically CamelCased). You finish the object definition later on with an end.

Most objects define a special method, initialize, that saves the initial data your object is created with (here, a radius) and performs any other required set-up.

You create an instance of your object with the new method. Arguments passed in to new are sent to your initialize method.

Data is stored on your object using instance variables that start with an @ sign. Instance variables behave like normal variables, but are only visible from inside a specific instance of your object. If you want the data to be externally accessible, you have to write more methods.