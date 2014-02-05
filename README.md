## Misc
* `CTRL+Q` - Turns on flow-control (if you turned it off by mistake)
* `CTRL+a` - increment number
* `:cw` - toggle quickfix list
* `CTRL+E` - scroll window down (cursor stays)
* `CTRL+Y` - scroll window up (cursor stays)
* `:r` - retrive (`:r filename` - loads file at cursor. `:r !ls` - loads ls at cur)

## Commands
* `:x` - exit (with save)
* `:e <path>` - open path
* `:w` - write (save)
* `:e!` - restore file (lose changes)
* `:saveas <path>` - save to new file
* `:edit` - open file in buffer

## Search/Find/Moving around
* `100G` - line 100
* `g;` - go back to last edit point (move back though changelist)
* `g,` - move forward through changelist
* `CTRL+o CTRL+i` - prev/next goto
* `two backticks` - go back to where you were
* `gi` - go back to last insert
* `gf` - load file under cursor
* `{, }` - prev, next paragraph
* `w` - start of next word (only alphanumeric + underscore)
* `e` - end of word
* `W` - start of next word
* `E` - end of word
* `%` - matching bracket
* `*` - next occurence of word
* `#` - previous occurence
* `fp` - find next `p`
* `Fp` - find previous `p`
* `tp` - `fp` but move cursor before
* `Tp` - `Fp` but move cursor before
* `,` - find next occurrence
* `;` - find previous occurrence
* `3fa` - find 3rd occurrence of `a`
* `^` - go to first non-space char on line
* `$` - end of line
* `?` - search backwards
* `:/s/old/new/g` - subtitue old for new
* `:1,10s/` - only between lines 1 and 10
* `:%s/` - whole file

## Editing
* `CTRL+r` - Redo
* `!!` - repeat last command
* `0y$` - yank from beginning to end of line
* `ye` - yank to end of line
* `dt"` - remove everything until `"`
* `CTRL+v` + move down - block select
* `I#ESC` - comment each line
* `CTRL+n` - complete word
* `CTRL+p` - complete word (previous)
* `X` - delete char to left of cursor
* `s` - delete char and enter insert mode

## Buffers
* `:ls` - list buffers
  * `a` - active
  * `#` - alternate buffer
  * `+` - buffer modified
  * `h` - hidden (unsaved changes and is not currently loaded in a window)
* `CTRL-^` - switch between active and alternate buffers
* `:bd!` - remove buffer (lossing changes)
* `:b22` - goto buffer 22
* `:b <match>` - goto buffer (tab to complete)

## Windows
* `ctrl-w w` - cycle between windows
* `:split` - split window or `sp`
* `:vsplit` - vertically split window
* `CTRL+w hjkl` - switch windows
* `CTRL+w c` - close window
* `CTRL+w n` - new window
* `CTRL+w s` - new split horizontally
* `ctrl+w v` - new split vertically
* `:sp <filename>` - split window and open fiename
* `:vsp <filename>` - split virtially and open filename
* `ctrl+w +/-` - resize windows

## Tabs
* `:tabe <file>` - open file in new tab
* `:tabedit <file>`
* `gt` - next tab
* `gT` - prev tab
* `2gt` - goto tab 2
* `:tabclose` - close all windows in current tab
* `:tabonly` - close all tabs execpt current one
* `ctrl-w T` - move current window into its own tab

## Macros
* `qa` - record actions in macro `a`
* `q` - end macro
* `@a` - playback `a`
* `@@` - playback last macro

## Spelling
* `[s`, `]s` - move to next/prev mispealt word
* `z=` - find suggested alternatives
* `zg` - add to dictionary
* `zw` - mark as misplealt

## Ruby and Rails
* `:Rake` - Run rake
* `:A [file]` - Alternate file/spec or load
* `:AS [file]` - As above but split horizontally
* `:AV [file]` - As above but split vertically
* `:AT [file]` - As above but open in new tab
* `:Elib [file]` - Edit lib file or Gemfile
* `:Espec [file]` - Edit spec file or spec_helper
* `:Ctags` - Ctags for the project
