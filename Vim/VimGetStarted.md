"=========== Meta ============
"StrID : 38
"Title : Vim Get Started
"Slug  : vim-get-started
"Cats  : Vim
"Tags  : 
"=============================
"EditType   : post
"EditFormat : markdown
"BlogAddr   : http://www.cguan.net/
"========== Content ==========
### GetStarted
First start with vimtutor. Run vimtutor in shell if you have installed vim. Here comes the vimtutor. Practice it step by step and I suggest study vimtutor multiple times.
Then, browser the help of vim. It provides some interesing tricks at the begining.
And then I learned vim by setting up some scenarios.
* Copy and paste?
Q1: How to select the text. 
A: Using visual mode. Press v at the begin of the text to be selected in normal mode and you will enter visual mode. Move cursor to select the text.
Q2: How to copy?
A: Just press 'y'.
Q3: How to paste?
A: Move the cursor to the point you want to paste the text to in normal mode. Press 'p'. The text is pasted to there.
Q4: Paste from clipboard?
A: Vim have multiple registers to copy and paste. The text in clipboard is also saved in registers. :reg will show you all the available registers and their values. :help p to see how to paste the text in certain register.

* Navigate between different files.
Q1: How to open files inside vim?
A: :edit [filename]. Vim will close current file and open target file. Filename can be auto complete with tab key. Filename also could be a directory. Vim will give out a list for you to select which file you want to edit. Actually, edit cmd does not close current. It is still in buffer. Use buffer to switch between files is much faster than normal way. [Here](http://joshldavis.com/2014/04/05/vim-tab-madness-buffers-vs-tabs/) is tutorial about how to use buffer and why use buffer.
Q2: How to edit two files in the same time?
A: :split and :vsplit will split the window into two part in vim.

* How to search in a project?
A: Use :grep to search. :copen will open a window called quickfix to show the result. Ack plugin is a better choice. I am still learning how to use Ack plugin.

### Using Plugin
I use Vundle to manage my plugins. Avoid usging plugins that need to be compiled seperately lik YouCompleteMe, Powerline.

### Vimscript
I learnt vimscript by "Learn Vimscript the Hard Way"[link](http://learnvimscriptthehardway.stevelosh.com).
