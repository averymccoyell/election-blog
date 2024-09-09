---
title: "Week 1"
author: "Package Build"
date: "2024-09-09"
output:
  word_document: default
  pdf_document: default
categories: []
tags: []
slug: "week-1"
---

# This is the first of weekly blog posts focused on predicting the results of the 2024 U.S. Presidential Election, as part of Professor Enos' GOV 1347: Election Analytics course. This blog will be updated on Mondays at 2pm. 


The upcoming U.S. Presidential Election has been dubbed by many as the most important election in history. Both Americans and people across the world see this November as a serious [test](https://foreignpolicy-com.ezp-prod1.hul.harvard.edu/2024/09/09/2024-us-election-harris-trump-democracy/) of democracy and the world order. Thus, it is all the more vital, for both sides, to accurately predict the results as best we can. However, there are several factors uniquely impacting this election which arguably make this [more difficult](https://corg.iu.edu/programs/hamilton-views/comments-on-congress/An%20Unprecedented%20Election%20%20And%20the%20Stakes%20Couldnt%20Be%20Higher.html) to do than ever before. The fact is, we are in an unprecedented election - after all, we've [never](https://cawp.rutgers.edu/facts/levels-office/federal-executive/women-presidential-and-vice-presidential-candidates-selected) had a woman of color (or a convicted felon, in the modern era) on a major-party ticket for President. Making this election all the more volatile was Biden's last minute drop-out just 3 months before the election, completely [changing](https://www.bbc.com/news/articles/c1e5xpdzkd8o) the race. Despite - and perhaps because of - all of these limiting and confounding factors, it remains incredibly important to continue predictions and analyses of this race. 

In this week's -- our very first -- blog post, we examine the *following two questions*: 

**1. How competitive are presidential elections in the United States?**
**2. Which states vote blue/red, and how consistently?**

First, we look at the competitiveness of presidential elections in the United States. 


<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-1-1.png" width="672" />

The graph above visualizes trends over time in two-party popular vote share by political party. In examining the graph, we can easily note that the popular vote share appears to be more evenly distributed between the two parties in recent years compared to earlier decades, where the two parties' popular vote shares simply seemed to follow a trend of flip-flopping by large margins every election. For example, the 2020 election had an approximate Republican share of 47.5% and Democratic share of 52.5% (5% margin), while the 1964 election had an approximate Republican share of 38% and Democratic share of 62% (24% margin). Thus, from the above graph we are able to determine that presidential elections in the United States (at least when considering two-party popular vote) are growing closer and more competitive. 

One could think of a few potential motivating factors behind this shift. Perhaps it is the rise of mass media and the 24/7 news cycle which has contributed, as the proliferation of campaign materials on media platforms allows for greater reach, visibility, and subsequent competitiveness. Along this line of thinking, perhaps the advent of targeted advertising online has allowed campaigns to more effectively persuade voters, resulting in tighter races. 

Either way, it is clear that by our metrics, presidential elections in the United States are becoming increasingly competitive. Now, let's zoom in - looking at states on an individual level, which tend to vote blue or red, and how consistently?


<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-2-1.png" width="1152" />
The above graph visualizes popular vote share by state, showing the country map color-coded by winning party for each presidential election since 1980. Taking a bird's-eye view, it does appear that aside from the 1980-88 period coinciding with the Reagan term, many states tend to remain consistent in their popular vote shares. For example, California, Washington, Oregon, Minnesota, New York, and New England at large have voted blue in every election since 1992. On the other hand, states like Texas, South Carolina, the Dakotas, Alabama, and Mississippi have voted red in every election since 1992. What this graph also shows us is those few states which tend to go back and forth, largely reinforcing common perceptions of "swing states" including Michigan, Nevada, Wisconsin, Pennsylvania, Arizona - even Ohio, Iowa, and Georgia, whose popular vote shares flip-flop between parties depending on the year. 

Now, having delved into the questions at hand, we end this week's blog post with a preliminary prediction for the 2024 election.


<img src="{{< blogdown/postref >}}index_files/figure-html/unnamed-chunk-3-1.png" width="672" />
The above graph offers a 2024 forecast using a simplified electoral cycle model wherein vote_2024 = 3/4*vote_2020 + 1/4*vote_2016. Each state is labeled by postal code, and is shaded by its predicted two-party popular vote margin (with higher numbers coinciding with a deeper red and a Republican advantage, and lower numbers coinciding with a deeper blue and a Democratic advantage). Thinking back to our previous discussion of swing states, my current prediction appears to give Harris a victory in Nevada, Michigan, and Pennsylvania, and hands North Carolina and Georgia to Trump. Arizona and Wisconsin remain unclear at this stage, with a predicted margin simply too close to tell. 

By considering the above predicted two-party popular vote margins for the 2024 Presidential Election by state, we are also able to offer a prediction on the electoral results. As seen below, that prediction currently stands at 276 electoral votes for the Democratic Party and 262 electoral votes for the Republican Party - *handing Kamala Harris the White House.* 




```
## # A tibble: 2 × 2
##   winner electoral_votes
##   <chr>            <dbl>
## 1 D                  276
## 2 R                  262
```

**Works Cited**

An Unprecedented Election – And the Stakes Couldn’t Be Higher: Comments on Congress: Hamilton’s Views: Programs: Center on Representative Government: Indiana University. (n.d.). Center on Representative Government. Retrieved September 9, 2024, from https://corg.iu.edu/programs/hamilton-views/comments-on-congress/An Unprecedented Election  And the Stakes Couldnt Be Higher.html

Hirsh, M. (2024, September 16). Is 2024 Really the Most Important Election in History? Foreign Policy. https://foreignpolicy.com/2024/09/09/2024-us-election-harris-trump-democracy/

Joe Biden drops out of election, upending race for White House. (n.d.). Retrieved September 9, 2024, from https://www.bbc.com/news/articles/c1e5xpdzkd8o

Women Presidential and Vice Presidential Candidates: A Selected List. (n.d.). Retrieved September 9, 2024, from https://cawp.rutgers.edu/facts/levels-office/federal-executive/women-presidential-and-vice-presidential-candidates-selected
