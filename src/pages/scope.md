
Variables have different scopes. Once the end of the scope is reached the values in that scope are no longer accessable

```ruby
def foo
  a = 10
end

puts a
# (file): undefined method `a' for main (NoMethodError)
```

**Global** variables do not need declarations. You simply assign a value to a global variable to create it.

```ruby
$b = 10
puts b
# 10
```

<route lang="yaml">
meta:
  title: Variable Scope
</route>
