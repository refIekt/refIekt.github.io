---
title: Migrating metadata
menubar: docs
---

{% include notification.html status="is-info" message="**Note**: Not yet implemented." %}

As you run your application metadata is created and stored in `db.js`.
If you then change a method or variable name, previously saved metadata will become outdated.
It's possible to rename classes and methods without losing past reflections.

## Renaming a class

Add the following inside your class:
```ruby
  reflekt_rename :class, :Tiger
```

## Renaming a method

Add the following inside your class:
```ruby
  reflekt_rename :meow, :roar
```

## Summary

Now when the program runs again, old reflections will be updated.
Once all reflections have been migrated `reflekt_rename` can be removed.
