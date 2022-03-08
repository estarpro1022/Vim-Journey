## Intro

### Modal editing

different operating modes:

* Normal
* Insert
* Replace
* Visual
* Command-line



keystrokes have different meanings in different operating modes.

The current operating mode will be shown in the bottom left.The initial/default mode is `Normal` mode.



You change modes by pressing `Esc` (the escape key) to switch from any mode back to **Normal mode**

From Normal mode, press `i` to enter Insert mode, `R` to Replace mode, `v` to Visual mode, `V` to Visual line mode, `<C-v>`(ctrl + v, sometimes ^v) to Visual block mode, `:` to Command-line mode.



### Basics

#### Buffers, tabs and windows

buffer: 缓冲区

tab: 标签页

window: 窗口

a vim session has many tabs, and a tab contains many windows. Each window shows a single buffer

一个vim会话有很多标签页

a given buffer may be open in multiple windows, even in the same tab. You can view different parts of file at the same time



By default, vim opens a single tab, which contains a single window



#### Command-line

In Normal mode, type `:` to enter Command mode.

This mode have functions such as opening, saving, closing, and quitting Vim

##### Some keystrokes

* `:q` to quit(close window)
* `:w` save
* `:wq` save and quit
* `:e {name of file}` open file for editing
* `:ls` show open buffers
* `:help {topic}` open help
  * `:help :w` open help for the `:w` command
  * `:help w` open help for the `w` movement



### Vim's interface is a programming language

> I expect muscle memory.

#### Movement

You spend most of time in Normal mode

* Basic movement: `hjkl` (left, down, up, right)
* Words: `w` (next word), `b` (beginning of word), `e` (end of word)
* Lines: `0` (beginning of line), `^` first non-blank character this line, `$` (end of line)

* Screen: `H` (top of screen), `M` (middle of screen), `L` (bottom of screen)
* Scroll: `Ctrl-u` (up), `Ctrl-d` (down) 默认滚动窗口数一半
* File: `gg` (beginning of file), `G` (end of file)

* Line numbers: `:{number}<CR>` or `{number}G` (line {number})
* Misc: `%` (corresponding item)
* Find: `f{character}`, `t{character}`, `F{character}`, `T{character}`
  * find/ to forward/ backward {character} on the current line
  * `,` / `;` for navigating matches
* Search: `/{regex}`, `n` / `N` for navigating matches



#### Edits

* `i` enter insert mode
* `o/O` insert line below/Above
* `d{motion}` delete, 
  * `dw` delete a word `d$` delete to the end of line `d0` delete to beginning of line

* `x` delete a character
* `s` substitute a character
* `u` to undo, `ctrl + r` to redo
* `y` to copy, `p` to paste

question:

`journey begin` when cursor lies in begin's b, then enter y, and paste it between blank of y and b, it paste blank, **why**



#### Counts

combine command with counts

* `3w` move 3 words forward
* `5j` move 5 lines down
* `7dw` delete 7 words



#### Modifier —— 修饰语





### Customized vim

vim is heavily customized, and it's worth exploring!!!!!





