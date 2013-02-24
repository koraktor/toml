# TOML

A sane configuration format from @mojombo.  More information here: https://github.com/mojombo/toml

## Usage

It's simple, really.

```ruby
content = <<-TOML

# Hello, this is an example.
[things]
other = "things"
what = 900000

TOML

parser = TOML::Parser.new(content)
# => { "things" => { "other" => "things", "what" => 900000 } }
```

## Contributors

Written by Jeremy McAnally based on TOML from Tom Preston-Werner.