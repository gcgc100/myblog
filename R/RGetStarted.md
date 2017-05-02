"=========== Meta ============
"StrID : 81
"Title : R GetStarted
"Slug  : r_getstarted
"Cats  : R
"Tags  : 
"=============================
"EditType   : post
"EditFormat : markdown
"BlogAddr   : http://www.cguan.net/
"========== Content ==========

R tutorial:
* [cyclismo R tutorial](http://www.cyclismo.org/tutorial/R/).
* [Quick-R](http://www.statmethods.net/index.html)

Install library: install.package("name")
R library:
ggplot2: A plotting system for R.
RMySQL: Database Interface and MySQL Driver for R.
```
library(RMySQL)
con <- dbConnect(MySQL(), user="root", password="password", dbname="dbname", host="localhost")
rs <- dbSendQuery(con, "sql")
data <- fetch(rs, n=-1)
dbClearResult(rs)
dbDisconnect(con)
```
