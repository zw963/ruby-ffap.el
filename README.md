ruby-ffap.el
======

This package make `ruby-mode` and `enh-ruby-mode` support `emacs-lisp-mode` FFAP(find file at point).

Installation
------------

Just drop ruby-ffap.el in your load-path and put the following in your .emacs
this package need [rvm.el](https://github.com/senny/rvm.el) to support it.

```lisp
(require 'ruby-ffap)

When use ido, following will enable fftp for ido:

```el
(setq ido-use-filename-at-point 'guess)
```

When use helm, following will enable fftp for helm

```el
(setq helm-ff-guess-ffap-filenames t)
```
```

Usage
-----

move you point over gem name.

e.g.

```rb
(require "fadaray")
```

When point over fadaray, press `Ctrl+x Ctrl+f`, will open file `your_gem_path/faraday-0.15.2/lib/faraday.rb` for example.

### Found a bug?

Please register a new issue.
