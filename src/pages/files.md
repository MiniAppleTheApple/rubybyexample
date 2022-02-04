```ruby
file = File.open "file-name"

# Get content of file

content = file.read

# Write the content to the file
file.write "#{content} writed into file"

# Commit the change
file.close
```

Rename

```ruby
File.rename "old-name", "new-name"
```

Get the size in byte of the file

```ruby
File.size "file-name"
```

Check if the file exist

```ruby
File.exist? "file-name"
```

Get the extension name from the file name

```ruby
File.extname "file-name.ext"
```

Get the file name without the directory part

```ruby
File.basename "dir/file-name"
```

Get the path for this file, without the file name

```ruby
File.dirname "dir/file-name"
```

Check if it's directory

```ruby
File.directory? "file-name"
```
<route lang="yaml">
meta:
  title: File IO
</route>
