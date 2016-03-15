Waf `:compiler` for Vim
=======================

Install
-------
Use your favorite plugin manager (I use pathogen)
```
$ cd .vim/bundle
$ git clone git@github.com/franc0is/vim-waf-compiler.git
```

Use
---
This plugin adds two compilers: `waf-build` and `waf-test`. Their behavior is
primitive:
* `waf-build` executes `pypy waf configure <args> build`
* `waf-test` executes `pypy waf configure <args> test`

Set either with `:compiler [compiler-name]`

and invoke them with `:make <args>`

Recommended plugins
--------------------
I use neovim. I found that [vim-dispatch](https://github.com/tpope/vim-dispatch),
with [the neovim extension](https://github.com/radenling/vim-dispatch-neovim) makes for
great user experience.
In that configuration, replace `:make` with `:Make`

