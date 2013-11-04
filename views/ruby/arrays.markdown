Arrays

Goals
Make some arrays and do stuff with them
Retrieve data from arrays
Step 1
Type this in irb:
fruits = ["kiwi", "strawberry", "plum"]
An array is a list of things in square brackets, separated by commas.

We generally call the individual things in an array elements.

Type this in irb:
things = [5, 'tree', 19.5]
things.length
An array can contain all sorts of things, not just strings.

length is a method that tells you how many elements are in an array.

Type this in irb:
  empty_array = []
  empty_array.length
The simplest kind of array is the empty array.

Step 2
Type this in irb:
fruits[0]
fruits[1]
fruits[2]
Array elements are stored in order. You can retrieve them by using the square brackets to access them by their index.

Arrays are ordered: elements remain in the same order they started in.

Ruby starts counting at zero: the first element is fruits[0].

Type this in irb:
fruits.first
fruits.last
Ruby gives us some helpful ways to get the first and last element from an array.

Step 3
Type this in irb:
['salt'] + ['pepper']
Arrays can be added together with the plus operator.

Type this in irb:
fruits + ['mango']
fruits
The plus operator doesn't modify the existing array, it makes a new one. How could you write that last piece of code to also modify the fruits array?

Step 4
Type this in irb:
fruits = ["kiwi", "strawberry", "plum"]
fruits.push('apple')
fruits.pop()
Ruby has many methods for modifying arrays. What did these two methods do?

Explanation
Arrays are used whenever you need to work with a large group of similar items.

A short list of methods for Array:

length  how long is this array (how many elements)
first get the first element of the array (same as array[0])
last  get the last element of the array (same as array[-1])
push  add a new element to the end of the array
pop remove (and return) the element at the end of the array
Further Reading
Ruby's documentation for Array
Next Step:
Go on to Hashes