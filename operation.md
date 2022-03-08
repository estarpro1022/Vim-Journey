## Operation

### basic
in the normal mode, we talk about specific operations here.

`x` delete the current character

`A` insert at the end of the line

`q!` force to exit 
`:wq` **save** and exit
`vim [document]` edit document

### delete command

`dw` delete from cursor to the beginning of next word, not include the first character 
`d$` delete to the end of the line
`de` delete to the end of the word

#### delete operation sign and operation object
`d motion` 
`dw` `de` `d$` `d0`

#### count
enter count in front of command
`2w` `3e`      
`0` move cursor to the beginning of line

##### delete more
`d number motion`
`d2w` 

##### operate whole line
`dd` delete the line
`2dd`/`d2d` delete two lines

##### revoke
`u` revoke final command
`U` revoke modification of whole line
`ctl+r` revoke the revoke command
hello
hello world
war


### insert command
`p` put final delete content to the back of cursor
`dd` to delete a line, then `p`, the line will occur next line


### substitute command
`r + [character]` to replace char at cursor

### modify
`c`
`ce` / `cw` change text to the end of word
test please
the difference between ce and de is that 
ce will enter **insert mode**, but de still maintain **normal mode** 

modify operator's mode is similar to delete operator.
`c [number] motion`
motion such as `w` `e` `$`

### fourth class

#### location and status
`ctrl + g` show the status
`G` to the end of document
`gg` to the beginning of document 
`[number] G` to the specified line

#### search
`/ + [string]`, press `n` to continue find, and press `N` to find in reverse order 
`? + [string]`, in a reverse order, press n to find the front character
`ctrl + o` (not 0) return former location----i'm not very clear
`ctrl + i` return the latest location

Ctrl + o ，在每一行有多个匹配字符串时，按Ctrl + o 回到上一行的最后一个匹配串，
Ctrl + i 则是下一行的最后一个匹配字符串，包括一行只有一个的字符串
#### 匹配括号
`%` 放在有括号的地方，光标跳到对应括号处, 也可以判断是否有不配对括号
(

#### substitute
`:s/old/new/g` replace `old` with `new` in the whole line
`:s/old/new` replace the first `old` in the current line with `new`


how to substitute every match string between two lines
`:[line number],[line number]s/old/new/g` 代表替换操作若干行中首尾两行序号

`:%s/old/new/g` replace every string in the entire doc
`:%s/old/new/gc` find doc's every string, and **ask whether to replace**


cambridge
cambol
cample
camp















