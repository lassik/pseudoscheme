# pseudoscheme
Scheme to Common Lisp

Using pseudoscheme:

The main issue is the readtable. To make it work with slime change to the scheme package in the listener

```lisp
(setq *readtable* ps::roadblock-readtable)
(in-package :scheme)
```
Then use slime eval functions. in the buffer you are editing in. 
slime-load-file doesn't work (yet).
