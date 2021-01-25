---
title: Configuration
menubar: docs
---

```ruby
Reflekt.configure do |config|

  # Reflekt is enabled by default and should be disabled on production.
  config.enabled = true

  # The amount of reflections to create per method call.
  config.reflect_amount = 5

end
```
