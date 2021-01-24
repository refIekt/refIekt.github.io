---
title: Usage
menubar: docs
---

Reflekt is designed to be super simple to use, all you have to do is `prepend` Reflekt to your class:

```ruby
class MyClass
  prepend Reflekt
end
```

In practice you will need to skip certain actions from being simulated. This stops duplicate data and prevent real data from being deleted.
