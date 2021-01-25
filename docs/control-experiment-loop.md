---
title: Control-Experiment loop
menubar: docs
---

Reflekt builds itself as you build your application.

**Terminology:**
* `Control` - A shapshot of real data (a subclass of `Reflection`)
* `Experiment` - A shapshot of random data (a subclass of `Reflection`)

**The loop:**
1. You write code and run it
2. A `Control` reflection is created per method call, tracking input and output
3. A set of rules are created from each `Control` on how the program works
4. Many `Experiment` reflections are created per method call, containing random input and output
5. Each `Experiment` is tested to pass or fail the set of rules previously defined by each `Control`
6. Results are saved to the `/reflections` directory
7. Your application returns its usual output

This feedback loop creates better results the more you develop and use your application.
