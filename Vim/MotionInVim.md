"=========== Meta ============
"StrID : 151
"Title : Move Cursor in Vim
"Slug  : move_cursor_in_vim
"Cats  : Vim
"Tags  : Vim motion
"=============================
"EditType   : post
"EditFormat : markdown
"BlogAddr   : http://www.cguan.net/
"========== Content ==========

Move inside one line:

* ^:First non-blank character; $:End of a line. Difficult to reach. I map them to H and L

1. Move forward:
    * l: Move one character
    * e: To next word begin
    * w: To next word end
    * t{char}: Till before  {char}
    * f{char}: To first {char}


2. Move backward:
    * h: Move one character
    * b: To next word begin
    * ge: To next word end
    * T{char}: same with t
    * F{char}: same with f


3. Up and Down:

    * j, k: up and down one line. I map j, k to gj, gk. When one line is too long and wrap by vim to two line, it's useful.
    * gg: first line
    * G: last line
    * {num}gg: to {num}th line
    * ctrl-u: Up half screen
    * ctrl-d: Down half screen
    * ctrl-b: Up one screen
    * ctrl-f: Down one screen

* Other:

    * M: Move the cursor to the middle of current window
    * zz: Scroll the screen to make current line in the middle of the window. Not move the cursor
