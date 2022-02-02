```ruby
age = 10
if age < 18 then
    puts "under 18"
end

# "then" is optional

age = 20
if age > 18
    puts "over 18"
elsif age == 18
    puts "is 18"
else
    puts "under 18"
end

unless age < 18
	puts "not under 18"
else
	puts "under 18"
end

puts "over 18" if age > 18
puts "is 18" if age == 18
puts "under 18" if age < 18
```

Comparison operators in Ruby:
```
==, <, >, <=, >=, !=
```

Combining Statements

```ruby
is_alive = false
age = 19
if is_alive and age > 18
    puts "good"
elsif not is_alive or age < 18 then
    puts "either dead or under 18"
end
```


<route lang="yaml">
meta:
  title: If/Else
</route>
