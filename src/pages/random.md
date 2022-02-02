```ruby
# Used to set a seed value for random.
srand Time.now.to_f

# random value between 0 tand 1
puts rand
# 0.6129308602771922

# random integer value from 1 to 100 (both inclusive)
puts rand 100
# 98

# random integer value from 20 to 100 (both inclusive)
puts (rand 100 - 20) + 20
# 54
```

<div class="border-2 rounded-md p-2 border-dashed border-gray-500">
<code>Time.now</code> has resolution down to seconds which means that if you invoke the command multiple times within a given second you'll get the same values back. You can try using more entropic sources for seeding like <code>/dev/random</code>.
</div>

<route lang="yaml">
meta:
  title: Random Numbers
</route>
