```ruby
module Greeting
	def hello
		puts "#{self} Sir"
	end
end

include Greeting

# Or hello
Greeting::hello
puts Greeting.class
```

```
Greeting Sir
Module
```

```ruby
module Foo
	def log
		puts "here is Foo"	
	end
end

module Bar
	include A
end

include Bar
Bar.log
```

```
here is A
```

```ruby
module Foo
	def log
		puts "here is Foo"
	end
end

module Bar
	def log
		puts "here is Bar"
	end
end

module FooBar
	include Bar
	include Foo
end

include FooBar

FooBar::log
```

```ruby
module Age
  def age
    @age
  end
  
  def age=(age)
    @age = age
  end
  
  def increment_age
    @age += 1
  end
end

module Runner
  def run
    puts "#{@name} is running"
  end
end
class Dog
  include Age
  include Runner
  def initialize(name, age)
		@name = name
		@age = age
  end
end

dog = Dog.new "Woof", 10

dog.age = 5
dog.increment_age
puts dog.age

dog.run

puts Dog.ancestors
```

```
6
Woof is running
Dog
Runner
Age
Object
Kernel
BasicObject
```

```ruby
module Age
  def age
    @age
  end
  
  def age=(age)
    @age = age
  end
  
  def increment_age
    @age += 1
  end
end

module Runner
  def run
    puts "#{@name} is running"
  end
end
class Dog
  extend Age
  extend Runner
  def initialize(name, age)
		@name = name
		@age = age
  end
end

Dog::run
puts Dog::age == nil

dog = Dog.new
dog.age
```

```
 is running
true
(file): undefined method `age' for #<Dog:0x7466 @name=nil @age=nil> (NoMethodError)
```

```ruby
module Foo
	def log
		super
		puts "Here is Foo"
	end
end

module Bar
	prepend Foo
	def log
		puts "Here is Bar"
	end
end

include Bar

Bar::log
```

```
Here is Bar
Here is Foo
```
<route lang="yaml">
meta:
  title: Module
</route>
