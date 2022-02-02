```ruby
greeting = "Hello, "
name = "Kenneth Sparks"
puts greeting + name

age = 19
name = "Laurence"
puts name + " is " + age + " years old"

hi = "Hi!"
puts hi.length # Alias hi.size
```
```
Hello, Kenneth Sparks
Laurence is 19 years old
3
```

We can create long strings and maintain white space

```ruby
long_string = "
I am a very very long
string that goes on for
ever"

puts long_string
```
```
I am a very very long
string that goes on for
ever
```

String formatting

```ruby
puts "not true = #{not true}"

# Or

puts "not true = $s" % (not true)
```
```
not true = false
```

<route lang="yaml">
meta:
  title: Strings
</route>
