# Preserve undo history after closing a file or exiting Vim

In your `.vimrc`:

`set undofile`

Now you can save and close a file in Vim, then realize you didn't need to do any of that work, and easily undo back to where you need to be!

## Bonus (but actually almost necessary)

In your `.gitignore_global`:

```
# Ignore all temporary files created by the Vim text editor
*~
```

All of vim's temporary files end with a tilde, so grab anything ending with a tilde and tell git to ignore it. If I run into any reason to specify, I'll let you know (or, you know, feel free to tell me).
