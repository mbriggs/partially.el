## partially.el - rails partial tools


I like small, focused libraries. This one provides some functionality
around rails partials. Supports erb and haml

```
partially/visit-partial     - jump to the partial rendered on the current line
NOT DONE!! partially/extract-partial   - extract a partial, dump it in a file, and render it in the current file
NOT DONE!! partially/inline-partial    - fetch the partial rendered on the current line, and replace the render statement with it
```

# Installation:

This relies on a "find-root" function. It defaults to railway-find-root (my standalone rails minor mode),
but can easily be customized to anything

```scheme
(setq partially:rails-root-fn 'rinari-root) ; use rinari function
(setq partially:rails-root-fn 'eproject-root) ; use eproject function
(setq partially:rails-root-fn 'projectile-get-project-root) ; use projectile function
(setq partially:rails-root-fn 'textmate-project-root) ; use textmate.el function
```