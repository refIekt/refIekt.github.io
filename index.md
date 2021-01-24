---
show_hero: true
title: Reflective testing
hero_icon: /assets/logo.svg
code_label: Usage
code: >
  ```ruby
    class Example
      prepend Reflekt
    end
  ```
callouts: callouts
---

Traditional testing is fine but it's not perfect. Tests often check for a golden path that works, when errors actually happen when the code or user does something unexpected. And with automated testing humans still have to write the tests.

**Reflekt** writes the tests for you, and tests in the negative for situations that you wouldn't have noticed. It works out of the box with no extra coding required. Because Reflekt tests your objects as they are used in the normal flow of the application, you get real world test results.
