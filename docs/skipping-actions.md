---
title: Skipping actions
menubar: docs
---

You can configure Reflekt to skip "no undo" methods like deletion and sending email:

```ruby
class ExampleClass
  reflekt_skip :method_name
```

## Databases

Use `reflekt_skip` on the method that saves to the database to avoid persisting test data. If you still want to save test data to the database then use [dependency injection](https://www.reddit.com/r/programming/comments/iz3rks/if_youre_not_practicing_within_the_scope_of_a/g6i1ex3/) to connect to a dummy database.

## Rendering to UI

Use `reflekt_skip` on methods that do the final render to the UI to avoid a visual mess of duplicated elements.
Separate the final output from the rendering logic so that Reflekt can track changes in output.

**Don't do:**
```ruby
def show(product)

  # Business logic.
  product.title = "Showing #{product.name}"

  # Rendering logic.
  puts product

end
```

**Do:**
```ruby
reflekt_skip :render

# Business logic.
def show(product)
  product.title = "Showing #{product.name}"  
  render(product)
end

# Rendering logic.
def render(product)
  puts product
end
```
