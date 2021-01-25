---
title: Getting Started
menubar: docs
---

## Installation

In your project's Gemfile add:
```ruby
gem 'reflekt'
```  

In terminal run:
```
bundle install
```

Or install globally with:
```
gem install reflekt
```

## Adding to your class

Reflekt is designed to be super simple to use, all you have to do is `prepend` Reflekt to your class:

```ruby
require 'reflekt'

class ExampleClass
  prepend Reflekt
end
```

In practice you will need to skip certain actions from being simulated, to prevent duplicate data from being rendered to the screen or saved to the database.

**Next:** [Skipping actions](/docs/skipping-actions)
