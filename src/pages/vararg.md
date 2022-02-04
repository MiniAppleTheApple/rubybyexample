Variable Arguments recieve unknown number of parameters as Array

```ruby
def get_sum(*args)
    sum = 0
	
	args.each do |arg|
		sum += arg
	end

    return sum
end

puts "Sum : #{get_sum(1, 2, 3, 4, 5, 6)}")
```
```
Sum : 21
```

<route lang="yaml">
meta:
  title: Variable Arguments
</route>
