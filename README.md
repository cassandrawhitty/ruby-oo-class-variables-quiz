# Quiz: Class Variables and Methods

## Class Variables and Methods

?: Classes are objects.
(X) True ( ) False

?: What type of scope does a class variable have?
( ) Local ( ) Global ( ) Instance (X) Class

?: What is the syntax for a class variable?
( )`@variable_name` (X)`@@variable_name` ( )`$variable_name` ( ) `VARIABLE_NAME`

?: 

```ruby
def self.class_method_name
  # some code
end
```

In this code sample, what does the keyword `self` refer to?
(X) The entire class itself  ( ) An instance of the class ( ) Local scope ( ) Instance scope

?: Private methods can only be called within the context of the defining class. The receiver of a private method is always `self`.
(X) True ( ) False

?: Private methods, including initialize, are usually written with the word "private" above them.
( ) True (X) False

?:

```ruby
class Book

  attr_accessor :name

  def initialize(name)
    @name = name
  end
end
```

What syntax should be used to to create a class variables that stores new instances of `Book` as soon as they're created?
( )
```ruby
class Book

  @@all = []

  attr_accessor :name

  def initialize(name)
    @name = name
  end
end
```
( )
```ruby
class Book
  attr_accessor :name

  def initialize(name)
    @name = name
    @@all << self
  end
end
```
(X)
```ruby
class Book

  @@all = []

  attr_accessor :name

  def initialize(name)
    @name = name
    @@all << self
  end
end
```
( ) None of the Above

?: What type of constant is defined within a class that are available to all instances of a particular class?
( ) Instance ( ) Local ( ) Global (X) Class

?: To create a class constant, what syntax should be used?
( )`@variable_name` ( )`@@variable_name` ( )`$variable_name` (X) `VARIABLE_NAME`

?: 
```ruby
class Book
  attr_accessor :author, :page_count, :genre
  attr_reader :title

  GENRES = []

  def initialize(title)
    @title = title
  end

  def turn_page
    puts "Flipping the page...wow, you read fast!"
  end

end
```

If a method requires some customization, what needs to change in the above code?
( ) Create the writer for genre and add the logic for the class constant ( ) Add an `attr_reader` for genre ( ) Remove the `attr_accessor` for genre (X) All of the Above

???