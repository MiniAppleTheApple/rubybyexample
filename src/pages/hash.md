```ruby
teams = {
    teamA: 12,
    teamB: 15,
}

puts teams["teamA"]

teams.each do |key, value|
	puts "#{key}:#{value}"
end
```

```
12
teamA:12
teamB:15
```

Insert

```ruby
teams["teamC"] = 1
```

Delete

```ruby
teams["teamA"] = nil
```

<route lang="yaml">
meta:
  title: Hash 
</route>
