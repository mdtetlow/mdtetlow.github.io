# Ruby

## Blocks

Multiple syntax options:

```ruby
do |something|
  #...
end

{ |something|
  #...
}


```

## Procs

```ruby
cheap = Proc.new do |price|
  price < 50
end  
```
All these are valid ways to call the proc:

```ruby
cheap.call(10)
cheap[10]
cheap.(10)
```

## Lambda

Note: Special type of Proc object

```ruby
cheap = lambda { |price| price <50 }
cheap.call(50)
```

Since Ruby 1.9 there are is a new syntax option
These are named "stabby" Lambdas due to the arrow!

```ruby
cheap = -> price { price < 50 }
#<Proc:0x0000000006a0cde0 (pry):22 (lambda)>
cheap[20]
```

Note: can wrap the parameter list in parenthasis if prefer and supports csv

```ruby
cheap = -> (price) { price < 50 }
cheap = -> price1, price2 { [price1, price2].min }
cheap[2, 4]
```

### Lambdas vs Procs

Call a Proc without an argument and it will use nil

Howver, call a Lambda without an argument and you get an `ArgumentError'.
This seems like the best behavour so favour Lambda over Proc


## useful commands

### methods

`block_given?` check if a block has been passed into the method

```ruby
def called_with_block
  if block_given?
    puts "Method has been passed a block"
  end
end
called_with_bloc? do
  1 + 2
end
```

`yield`

```ruby
def print_and_yield
  puts "print a message"
  yield
  puts "print another message"
end

print_and_yield do
  puts "my message"
end
```

```ruby
def map_words(input)
  results = []
  input.split.each do |word|
    results << yield(word)
  end
  results
end

map_words("My name is Mark") do |word|
  word.size
end
```
