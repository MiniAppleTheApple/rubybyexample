[Environment variables](http://en.wikipedia.org/wiki/Environment_variable) are a universal mechanism for [conveying configuration
information to Unix programs](http://www.12factor.net/config).

```ruby
secret = ENV["SECRET"]
puts "SECRET not set" if secret
puts secret
```

```bash
$ SECRET=12345 ruby envtest.rb
12345
```

<route lang="yaml">
meta:
  title: Environment Variables
</route>
