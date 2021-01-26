---
title: Configuration
menubar: docs
---

To configure Reflekt call `Reflekt.configure` and modify a property on the `config` block parameter:

```ruby
Reflekt.configure do |config|
  config.enabled = true
end
```

#### enabled

```ruby
config.enabled = true
```
Reflekt is enabled by default and should be disabled on production.

#### git_ignore

{% include notification.html status="is-info" message="**Note**: Not yet implemented." %}

```ruby
config.git_ignore = true
```
Reflekt is untracked in git by default.

#### reflect_amount

```ruby
config.reflect_amount = 5
```
The amount of reflections to create per method call. A control reflection is created in addition to this.

#### reflect_limit

```ruby
config.reflect_limit = 10
```
The maximum amount of reflections that can be created per instance/method. A method called thousands of times doesn't need that many reflections.

#### project_path

```ruby
config.project_path = nil
```
An absolute path to the project root directory. Defaults to current execution path.

#### output_directory

```ruby
output_directory = "reflections"
```
Name of output directory.
