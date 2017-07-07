"=========== Meta ============
"StrID : 139
"Title : Aliases
"Slug  : aliases
"Cats  : shell
"Tags  : zsh
"=============================
"EditType   : post
"EditFormat : markdown
"BlogAddr   : http://www.cguan.net/
"========== Content ==========

I start to learn zsh these days.
This is what I got about aliases.

* Aliases expand into some other text and are used as a command. 

* Normal aliases only work when in command position. Use '-g' option to alias to create global aliases so that it can be expanded in anywhere. 

* The aliases can contain something of the same name as it self. e.g.

  > alias mkdir='nocorrect mkdir'

  the *mkdir* inside the alias will not be expanded.

* Aliases can not take arguments.
