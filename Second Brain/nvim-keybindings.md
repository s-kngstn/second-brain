# [[nvim]] keybindings
## Current most common vim movements
### Netrw
vim . = go to curr directory filepath
% = create new file
d = create new directory
:Ex = explore directory tree
:Sex! = explore directory tree in side window
:so = source current file

### Project Navigation

**Open current directory (Netrw)** `<space> + pv`

**Search for file / fuzzy finder** `<space> + pf`

**Search / fuzzy find recent Buffers** `<space> + pb`

**Search / grep word or words within project**  `<space> + ps`

**Close Search file / fuzzy finder** `esc`

**Toggle Terminal** `<CTRL> + \`


### Window Split & Movement

**Split Page Vertically** `<CTRL> + s`

**Close Split** `Same as save and quit or no save and quit... :wq or :x`

**Go to definition**  `<space> g + d`

**Navigate windows**

⬅️ Switch to the left window  `<ctrl> + h`
➡️ Switch to the right window  `<ctrl> + l`
⬆️ Switch to the top window  `<ctrl> + k`
⬇️ Switch to the bottom window  `<ctrl> + j`

## Movements
Movements in vim are best used in combination with:
**Command | Count | Motion**
Commands = d (delete), c (change/delete & insert), y (copy/yank), v (visual), f (forward to letter on current line e.g fs takes you to the first "s")
Count = The relative line number on the page (the destination)
Motion = See motions / movements below

Examples of **CCM** (Command | Count | Motion)

**Jump 5 lines down**
	- Count: 5
	- Motion: j (down in vim)

### Horizontal Movements
**Beginning of line**  `0`
**First char of line**  `_`
**Last char of line**  `$`
**Go to forward char on line** `f (forward) + <character>` eg: `fg`
**Go to backward char on line** `F (back) + <character>` eg: `Fg`
`;` will then let you hop to the the next like character on the line
`,` will let you hop back to the previous like character on the line
**Delete until char** `dt"`

### Vertical Movements
**Top of page** `gg`
**Bottom of page** `G`
**Big hop down page** `<CTRL> + d`
**Big hop up page** `<CTRL> + u`
**Num lines up** `<line number> + k`
**Num lines down** `<line number> + j`

**Hop through same words on page** 
	go to beginning of word you want then `*` grabs the word
	you can then use 
		`n` to go to the next
		`N` to go to the previous

### Edit Movements
**Copy 5 lines up** `y5k`
**Copy 5 lines up** `y5j`
**Delete 5 lines up** `d5k`
**Delete 5 lines down** `d5j`

**Change Code within Curly Braces {}**  `c + i + {`

**Highlight and move code chunks** 
	1. in visual-line mode `<shift> + v` highlight the code you want to move.
	2. Up: `<shift> + k` Down: `<shift> + j`
	3. Left: `<` Right: `>`


## Diagnosis 

### toggle relative line numbers `<leader> + r`



**Hover document**  `<shift> + k`

**Toggle relative line numbering**  `<space> + un`

**Go to line number** `<number of line> + G`

**Search and Replace all words in a file** `:%s/oldword/newword/g`

Ctrl + w q

Go to begining of line 
0

Go to end of line
$

Copy and yank multiple lines
Go to end of current line you wish to copy
Ctrl + v
Go up to last line you wish to copy
y
then navigate to where you wish to paste the code and press 
p
