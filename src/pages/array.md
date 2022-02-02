```ruby
colors = ["red", "green", "blue"]


puts "With positive index: #{colors[0]}, #{colors[1]}, #{colors[2]}"

puts "With negative index: #{colors[-1]}, #{colors[-2]}, #{colors[-3]}"

puts "Number of items: #{colors.size}"
```


```
With positive index: red, green, blue 
With negative index: blue, green, red
Number of items: 3
```

```ruby
colors = ["red", "green", "blue"]

colors.each_with_index do |color, i|
	puts "#{i + 1}:#{color}"
end
```

```
1:red
2:green
3:blue
```
Append to the end of the table
```ruby
colors = ["red", "green", "blue"]

colors.push "orange"

index = colors.length

puts colors[index - 1]
```

```
orange
```
Insert at index
```ruby
colors = ["red", "green", "blue"]

colors.insert 2, "pink"

puts colors.join "\n"
```

```
red
green
pink
blue
```

Remove

```ruby
colors = ["red", "green", "blue"]

colors.drop 1 

puts colors.join "\n"
```

```
green
blue
```
<route lang="yaml">
meta:
  title: Array 
</route>
