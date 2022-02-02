You can assign any value to any variable

```ruby
x = "I love ruby" # String
x = 10            # Integer
x = 6.7           # Float
x = true          # TrueClass
x = false         # FalseClass

require "set"

x = [1, "Hello", 3.14, false, true] # Array
x = Set.new [1, 2, 3]               # Set
x = {:foo => 1}                     # Hash
```

There is no variable keyword, but...

```ruby
local = 10         # local variable
CONSTANT = "Hello" # constant warn when change it
$global = true     # global variable
```

You can't use undefined variable

```ruby
puts x
```
<route lang="yaml">
meta:
  title: Variables
</route>
