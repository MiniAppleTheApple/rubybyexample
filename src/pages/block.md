```ruby
l = [1, 2, 3, 4, 5].map {1}
puts l.join ", "
```

```
1, 1, 1, 1, 1
```

```ruby
l = [10, 20, 30]

l.each {|i| puts i}
```

```
10
20
30
```

```ruby
l.each do |i|
	puts i + 10
end
```

```
20
30
40
```
<route lang="yaml">
meta:
  title: Block
</route>
