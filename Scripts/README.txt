Given an input year, this crawler will return the following fields from every article 
published in the Journal from "input year" to December 2019 (last listed publication):

Title
Author
Author Affiliations
Correspondence Email
Publication Date
Abstract
Keywords

#Full Text

The r.md file includes code for parsing the full article text as well.
However, when run for multiple years, the R session crashed and I did not have enough time
to correct the issue. However, the code can be run for one year including the full article 
text.

Essentially, given the input year, the Crawler connects to the publication site for that year
and uses a for loop to crawl the site for every article, of every issue of every year since
the input year.

All the code is collected into a single R file. 

For example, the program can be run as:

> Crawler(2017)

To parse the journal for every year since 2017, including 2017.