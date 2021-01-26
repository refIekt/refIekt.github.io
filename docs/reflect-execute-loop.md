---
title: Reflect-Execute loop
menubar: docs
---

Reflekt is designed to be used without custom coding and with as little configuration as possible. That being said, you may be interested in understanding how Reflekt actually works.

Reflekt wraps itself around your code, reflecting it, then returns control to the application to continue its original execution. This process is called the Reflect-Execute loop because it happens via a single function that changes behaviour depending on what stage the loop is in.

## Terminology

* `Action` - An action represents an event such as a method being called

## The loop

1. `Reflekt` is prepended to a class and setup
2. The method is overridden on class instantiation
3. An `Action` is created on method call
4. Many `Refections` are created per `Action`
5. Each `Reflection` executes on cloned data
6. Flow is returned to the original method
