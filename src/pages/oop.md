<route lang="yaml">
meta:
  title: OOP
</route>

```ruby
class Dog 
	def initialize(name, age)
		@name = name
		@age = age
	end

	def run
		puts "#{@name} is running"
	end
end

dog = Dog.new # Or Dog::new
dog.run
```

```
Woof is running
```

You can't access any attribute directly from Dog object, you need `setter` and `getter`

```ruby
puts dog.age
```

```
file): undefined method `age' for #<Dog:0x562c @name="Woof" @age=10> (NoMethodError)
```

Create setter and getter by yourself

```ruby
class Dog
	def initialize(name, age)
		@name = name
		@age = age
	end
	
	# The getter
	def age
		@age
	end
	
	# The setter
	def age=(age)
		@age = age
	end

	def run
		puts "#{@name} is running"
	end
end
dog = Dog.new "Woof", 10
dog.age = 5
puts dog.age
```

```
5
```

`attr_acessor`

```ruby
class Dog
	attr_accessor :age
	def initialize(name, age)
		@name = name
		@age = age
	end

	def run
		puts "#{@name} is running"
	end
end
dog = Dog.new "Woof", 10
dog.age = 5
puts dog.age
```

```
5
```
`attr_reader`

```ruby
class Dog
	attr_reader :age
	def initialize(name, age)
		@name = name
		@age = age
	end

	def run
		puts "#{@name} is running"
	end
end
dog = Dog.new "Woof", 10
dog.age = 5 # You can't write
puts dog.age
```

```
(file): undefined method `age=' for #<Dog:0x7bc @name="Woof" @age=10> (NoMethodError)
```

`attr_writer`

```ruby
class Dog
	attr_writer :age
	def initialize(name, age)
		@name = name
		@age = age
	end

	def run
		puts "#{@name} is running"
	end
end
dog = Dog.new "Woof", 10
dog.age = 5
puts dog.age # You can't read 
```

```
(file): undefined method `age' for #<Dog:0x836 @name="Woof" @age=5> (NoMethodError)
```

```ruby
class Automotive
  def initialize(speed, capacity)
    @speed = speed
    @capacity = capacity
  end
  
  def move
    puts "moving in #{@speed}km/h"
  end
  
  def enough_space?(space)
    return space < @capacity
  end
end

class Car < Automotive
  def initialize
    super 100, 5
  end
end

class Bus < Automotive
  def initialize
    super 80, 20
  end
end
car = Car.new
car.move
puts car.enough_space? 4

bus = Bus.new
bus.move
puts bus.enough_space? 24
```

```
moving in 100km/h
true
moving in 80km/h
false
```
