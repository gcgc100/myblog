"=========== Meta ============
"StrID : 180
"Title : Use Mutt To Receive And Send Email
"Slug  : use-mutt-to-receive-and-send-email
"Cats  : shell
"Tags  : email shell
"=============================
"EditType   : post
"EditFormat : Markdown
"BlogAddr   : http://www.cguan.net/
"========== Content ==========

sudo apt-get install mutt

sudo touch /var/mail/$USER
sudo chmod 660 /var/mail/$USER
sudo chown \`whoami\`:mail /var/mail/$USER

Create ~/.muttrc file

>
set realname = "<first and last name\>"
set from = "<gmail username\>@gmail.com"
set use_from = yes
set envelope_from = yes
>
set smtp_url = "smtps://<gmail username\>@gmail.com@smtp.gmail.com:465/"
set smtp_pass = "<gmail password\>"
set imap_user = "<gmail username\>@gmail.com"
set imap_pass = "<gmail password\>"
set folder = "imaps://imap.gmail.com:993"
set spoolfile = "+INBOX"
set ssl_force_tls = yes
>
\# G to get mail
bind index G imap-fetch-mail
set editor = "vim"
set charset = "utf-8"
set record = ''

m to start sending new messages.
G to fetch new messages.

Source: [http://nickdesaulniers.github.io/blog/2016/06/18/mutt-gmail-ubuntu/](http://nickdesaulniers.github.io/blog/2016/06/18/mutt-gmail-ubuntu/)
