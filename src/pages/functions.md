```ruby
def calculate_tax(price)
    return price * 0.21
end

def sum(a, b = a)
	a + b
end

result = calculate_tax (sum 50) 
puts price
```
```
21
```

```ruby
def info name, age, country
	puts "#{name} is #{age} years old"
end

info "Kenneth", 12, "Jupiter" 
```
```
Kenneth is 12 years old.
```

```ruby
def block_sum
	yield + yield
end

puts block_sum {10}
```

```
20
```
<route lang="yaml">
meta:
  title: Functions
</route>
