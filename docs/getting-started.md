---
title: Getting Started
menubar: docs
---

{% include notification.html status="is-info" message="**Note**: Do not use Reflekt on a live site." %}

## Installation

In your project's Gemfile add:
```ruby
gem 'reflekt'
```  

Then in your terminal run:
```
bundle install
```

Or install globally with:
```
gem install reflekt
```

## Adding to your class

All you need to do is `prepend` Reflekt to your class:

```ruby
require 'reflekt'

class ExampleClass
  prepend Reflekt
```

However you should skip certain actions from being simulated, to prevent duplicate data from being rendered to the screen or saved to the database.

**Next:** [Skipping actions](/docs/skipping-actions)
