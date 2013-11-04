# Hashes

## Goals

- Make some hashes and get data back out of them
- Understand why we might use a Hash
- Understand the differences between Arrays and Hashes

### Step 1
Type this in irb:

```ruby
states = {"CA" => "California", "DE" => "Delaware"}
```

An array just stored items in some order. A hash stores pairs of items, associating *keys* with *values*.

The `{` character is typically called a 'curly brace', and the `=>` is called a 'rocket' or 'hashrocket'

Type this in irb:

```ruby
states.keys
states.values
```

You can ask a hash for an array of just its keys or its values.

Type this in irb:

```ruby
states['CA']
states['DE']
```

With arrays, we accessed elements by their *index*, a number. With a hash, we access elements by their *key*.

### Step 2

Type this in irb:

```ruby
  bike1 = {'make' => 'Trek', 'color' => 'Silver'}
  bike2 = {'make' => 'Cannondale', 'color' => 'Blue'}
  bikes = [bike1, bike2]
```

Hashes are often used to store the properties of some object. Here, each hash stores the properties of a bike.

The *keys* are often the name of a property (here *make*, *color*) while tha values are the value of the property for a given object (here, *Trek*, *silver*).

Consider how you might have had to store this data if you didn't have hash. What else might you want to store in a hash?

Type this in irb:

```ruby
  bikes[0]['make']
  bikes[1]['color']
```

When objects are nested deeply in arrays and hashes, you can access elements one after the other like this.

For example, on the first line here, we are getting the first *bike* in the *bikes* array (`bikes[0]`) and then getting its *make* (`bikes[0]['make']`)

##Explanation

Hashes are a fundamental way to group large amounts of related data. In other languages, hashes are called *dictionaries*, *maps*, or *associative arrays*.

## Further Reading

Ruby's documentation for [Hash](http://www.ruby-doc.org/core-1.9.3/Hash.html)

Next Step:
Go on to [Loops](loops)
