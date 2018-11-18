### rack
---
http://rack.github.io/

```ruby
require 'rack'
app = Proc.new do |env|
  ['200', {'Content-Type' => 'text/html'}, ['A barebones rack app.']]
end
Rack::Handler::WEBrick.run app

# config.ru
run Proc.new { |env| ['200', {'Content-Type' => 'text/html'}, ['get rack\'d'']] }
```

```sh
rackup config.ru
```

```
```


