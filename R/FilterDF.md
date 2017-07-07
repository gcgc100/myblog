"=========== Meta ============
"StrID : 120
"Title : Filter Data Frame
"Slug  : filter-data-frame
"Cats  : R
"Tags  : 
"=============================
"EditType   : post
"EditFormat : markdown
"BlogAddr   : http://www.cguan.net/
"========== Content ==========

I try to filter data frame by the group count of multiple columns.

Combine multiple columns together, calculate the count and filter the dataframe by the count.

I did not find an easy way to do this. I use table to calculate the count and filter the dataframe by *apply* function.
>
\> df <- data.frame('a'=c(1,1,2,2,3,3,3), 'b'=c(1,2,2,2,4,3,3))
\> df
  a b
1 1 1
2 1 2
3 2 2
4 2 2
5 3 4
6 3 3
7 3 3
>
\# Filter code
\> tempTable <- table(df$a, df$b)
\> check <- function(x, a, b) { 
    return(tempTable[toString(x[a]), toString(x[b])] != 2)
}
\> df <- df[apply(df, 1, check, a="a", b="b"), ]
\# Filter code end
>
\> df
  a b
1 1 1
2 1 2
5 3 4
>
