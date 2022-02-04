### While

```ruby
i = 1
while i <= 10 do # "do" is optional
	if i < 3
		break
	end
	puts i
	i = i + 1

	# break throws you out of a loop
	if i == 8 
		break
	end
end
```
```
3
4
5
6
7
```

### Until 

```ruby
guess = 0
# Convert String to Integer
until guess.to_i == 15
	print "Enter your guess: "

	# Gets input from the user and removes carriage return characters
	guess = gets.chomp
end
```

### Begin
```ruby
i = 0
begin
	puts i
	i += 1
end while i < 10

# Or

i = 0
begin
	puts i
	i += 1
end until i > 10
```

### For

```ruby
# start..end
for i in 0..10 do
	puts i 
end
```
```
0
1
2
3
4
5
6
7
8
9
0
1
2
3
4
5
6
7
8
9
```

### Loop methods

```ruby
10.times {|i| puts i}
```

```
0
1
2
3
4
5
6
7
8
9
```


```ruby
["Hello", "Jason"].each {|i| puts i}
```

```
Hello
Jason
```

```ruby
{foo: true, bar: false}.each {|key, value| puts "#{key}:#{value}"}
```

```

foo:true
bar:false
```

<route lang="yaml">
meta:
  title: While/For
</route>
