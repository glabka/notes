# vim
* i - insert mode
* r[character] - replaces a current character with {character}
* ecs - escape to normal mode
* . - repeat last command
* ; - repeat f or t command
* u - undo
* ctrl + r - redo
* o - add line bellow and go to insert mode
* O - add line above and go to insert mode
* S - delete line and enter insert mode
* p - paste after the cursor
* P - paste before the cursor
* "+p - paste from ubuntu system clipboard
## moving around
* h / j / k / l - move around in normal mode
* /[text] - to find and go to [text], press n to go to  next occurrence, N to go to previous one
* ?[text] - to find and go to previous occurrence of [text]
* f[character] / F[character] - go to next / previous [character] in line
* t[character] / T[character] - go to next / previous [character] in line, cursor set before this {character}
* H / M / L - go to highest/middle/lowest line on screen
* [number]% - go to [number] percent of file
* w / W - go to beginning of the next word (punctuation considered a word / words are separated by spaces)
* e / E - go to end of the next word (punctuation considered a word / words are separated by spaces)
* b / B - go to beginning of previous word (punctuation considered a word / words are separated by spaces)
* ge - go to end of the previous word
* ^ - go to beginning of line
* $ - go to end of line
* gg - go to beginning of file
* G - go to last line
* [number]G - go to line of number [number]
* * - go to next occurrence of the word under cursor
* # - go to previous occurrence of the word under cursor
## operators
* d - delete
* dw - delete up to end of the next word
* de - delete up to beginning the next word
* d[number]b - delete [number] of to the left of cursor
* dd - delete line
* d0 - delete from cursor to begginning of line
* d$ - delete from cursor to end of line
* [number]yw - copy next [number] of words
* c% / d% / y% - delete and copy / delete end copy / copy all upcoming characters with opening and ending of special characters like parenthesis e.g. copy "equivalent(entry.key(), qk.key)"
* ci" - delete and copy everything inside the ""
* yaB - copy everything within brackets a bracket block included
* df[character] - delete everything until the [character] including the character
# other commands
* zt / zz / zb - fix cursor and scroll text to top / center / bottom
* ma + d'a - set mark a at current location (then move to different line) + delete from current line to line mark a
* >aB - auto reindent a block
# command-line mode
* :s/regex/text/g - substitute all matches from regex with text in current line. (in begginning of regex write \v for 'very magic' for special characters and escaping to work as I know it from java)
* :help [command] - help page for command
* :wq! - force (because of !) the (w)rite and (q)uit
