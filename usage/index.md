---
title: Usage
menubar: docs
---

Reflekt is designed to be super simple to use, all you technically have to do is `prepend` Reflekt to your class:

{% highlight ruby %}
class MyClass
  prepend Reflekt

  # Your yummy code here...
end
{% endhighlight %}

In practice you will need to skip certain actions from execution to stop duplicate data and prevent real data from being deleted.
