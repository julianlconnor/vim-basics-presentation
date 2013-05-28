#How to not be a `scrub`.. AKA Vim Basics

## What is `Vim`?
`Vim` is a highly configurable text editor built to enable efficient text editing. It is an improved version of the `vi` editor distributed with most `UNIX` systems.

`Vim` is often called a "programmer's editor," and so useful for programming that many consider it an entire `IDE`. It's not just for programmers, though. `Vim` is perfect for all kinds of text editing, from composing email to editing configuration files.

## Why `Vim`?
- Ubiquitous use at Venmo, except for a few outsiders/scrubs.. ;)
- Fast, lightweight, very customizable and extensible.
- It's a text EDITOR not processor. Navigating through code in an efficient manner saves LOTS of time.
- When you become fluent in Vim's ways, muscle memory starts to take over and you stop thinking and start doing like an improvising musician.
- Basic Modes: `Normal`, `Insert`, `Visual`.
    - `Normal`: used for navigating and maniuplation of text.
    - `Insert`: used for adding new text.
    - `Visual`: for navigation and manipulation of text selections.

## How do I `Vim`?
- Make sure to learn incrementally.
    - You WILL fail if you attempt to dive into the deep end before learning to swim.
- Don't know the best shortcut for achieving fame at Venmo? Ask someone / look it up. :D
- Start with a fresh `Vim` configuration and slowly customize it to your needs.

## The Zen of `Vim`
- You're speaking a language when using `Vim`. The language is spoken in `‘verb modifier object’` sentences turned into acronyms.
- `Verbs`: `v` (visual), `c` (change), `d` (delete), `y` (yank/copy).
- `Modifiers`: `i` (inside), `a` (around), `t` (till.. finds a character), `f` (find, similar to `till` but is inclusive), `/` (search).
- `Objects`: `w` (word), `s` (sentence), `p` (paragraph), `b` (block), `t` (tag, works for html/xml).

### Using these `verbs`, `modifiers`, and `objects`- try to speak to `Vim`.
- delete the current word
    - `diw` (delete inside word).
- change current sentence
    - `cis` (change inside sentence).
- change a string inside quotes
    - `ci"` (change inside quote).
- change html inside of tag
    - `cit` (change inside tag).
- difference between change and delete is that change will put you in insert mode.
- you get the point.. :)

## Movement
- `h`, `j`, `k`, and `l`
    - as essential as `wasd` for all you gamers.
- More Advanced
    - `w` and `W`
        - `w` jumps by start of words, punctuation is considered
        - `W` jumps by words, delimited by spaces
    - `e` and `E`
        - `e` jumps to end of words, punctuation is considered
        - `E` jumps to end of words, delimited by spaces
    - `b` and `B`
        - `b` jumps backwards by words, punctuation is considered
        - `B` jumps backwards by words, no punctuation
    - `^` and `$`
        - `^` jumps to the first non-blank character on the line
        - `$` jumps to the end
    - `f` and `F`
        - find character on line, `f` is infront, `F` is behind
        - `;` will jump to the next instance
    - `/` and `?`
        - `/` searches below the cursor
    - `?` searches above
        - once search has been made: `n` and `N`
            - `n` repeats search in same direction
            - `N` repeat search in opposite direction
    - `i` and `I`
        - `i` jumps into insert mode at the current location
        - `I` jumps into insert mode at the beginning of the line
    - `a` and `A`
        - `a` jumps into insert mode at the end of the current word
        - `A` jumps into insert mode at the end of the current line
    - `esc`
        - exit `insert` mode :)

## Editing
- `r` (I JUST LEARNED THIS TODAY LOL)
    - replaces a single character WITHOUT going into insert mode, super clutch.
- `J` 
    - joins the line below with the current one
- `s` and `S`
    - `s` deletes the character at the cursor and goes into insert mode, similar to r
    - `S` deletes the line at the cursor 

## Exiting
- `:w`
    - write file but don't quit
- `:wq`
    - write file and quit
- `:q`
    - quit, will fail if there have been changes since last save
- `:q!`
    - force quit

## Working with multiple files
- `:vs` and `:sp`
    - `:vs` creates a vertical split
    - `:sp` horizontal

## Plugins
- `Command-T`, `Ctrl + P`
- `Nerd Tree`
- `Git Fugitive`
- `PyFlakes`
- `Snipmate`

## Pro-Tips
- . will repeat previous command
- gf will open a file path in a new buffer, demo
- '. will jump to the last edited line
- ctrl + o will jump to the previously visited location
- macros!

# Questions & Exercise
- Sorry for the info dump.


