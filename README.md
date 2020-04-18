# phpbot.el

## Overview

Emacs package to assist in PHP development

## Usage 

1. Check that the popup-el is loaded. [popup-el](https://github.com/auto-complete/popup-el) 

2. Config .emacs

```lisp
(add-to-list 'load-path "~/.emacs.d/site-lisp/popup-el")

(require 'phpbot)

(custom-set-variables
 '(phpbot-bin-path "/Users/coleflowers/antlr/build/phpbot"))

```

3. You can use phpbot.el in any of the following ways

- Direct Binding Shortcuts

```lisp
(define-key php-mode-map (kbd "M-/")
 'phpbot-gettersetter)
```

- Pop Menu

```lisp
(define-key php-mode-map (kbd "M-/")
 'php-generator-menu)
```

## Screenshots

**popup menu**

![](https://raw.githubusercontent.com/thinkcn/phpbot.el/master/screenshot/phpbot-el-menu.png)