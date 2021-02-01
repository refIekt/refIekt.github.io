---
title: Lit CLI
subtitle: Shine a light on terminal commands.
show_hero: true
---

<p align="center">
  <a href="https://www.mozilla.org/MPL/2.0/" alt="MPLv2 License">
    <img src="https://img.shields.io/badge/license-MPLv2-blue.svg" />
  </a>
  <a href="https://rubygems.org/gems/lit-cli">
    <img src="https://badge.fury.io/rb/lit-cli.svg" alt="Gem Version" />
  </a>
</p>

*Shine a light on terminal commands.* 🔥

Lit is Reflekt's command line interface that lets you view metadata generated as an application runs.

## Usage

Simply start any command with `lit`.

`rails server` becomes:
lit rails server
```

`ruby script.rb` becomes:
```
lit ruby script.rb
```

## Installation

Run:
```
gem install lit-cli
```

Applications using the Lit API will install the `lit` command for you.

## Integrate with Lit

To integrate your application see the [Lit API](https://github.com/lit-cli/lit-api).
