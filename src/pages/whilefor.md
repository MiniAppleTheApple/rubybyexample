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

i= 0
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
1
2
3
4
5
6
7
8
9
1
0
```

<route lang="yaml">
meta:
  title: While/For
</route>
