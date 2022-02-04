Using code from another file

<div class="grid grid-cols-2 gap-2 lt-sm:grid-cols-1">

```ruby
# main.rb
require_relative "info"

value_of("John")
```

```ruby
# info.rb 
def value_of(x)
	puts "Value of: #{x}"
end
```

</div>

```bash
$ ruby main.rb
Value: John
```

<route lang="yaml">
meta:
  title: Require
</route>
