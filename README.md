# prj_example_data

Some example data for use with example code. Use with `RCurl` e.g.

```r
library(RCurl)
library(magrittr)
countData <- getURL("https://raw.githubusercontent.com/Perugolate/prj_example_data/master/part_rep.ex.dat.tsv") %>% 
  textConnection %>% read.table %>% round
countDesc <- getURL("https://raw.githubusercontent.com/Perugolate/prj_example_data/master/part_rep.ex.col.tsv") %>% 
  textConnection %>% read.table(header=FALSE)
```
