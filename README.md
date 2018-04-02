### Marketing-Analysis-w-R
**Introduction of data set:**<br>
  This data set is prepared for analyzing the impact of an automotive brand competitors' keyword bidding strategy. In order to focus on the competition performance, this data includes the segment, make, and model of the competitve vehicle, the geographic (region and market) for each observation, competitor's vehicle sales, price, incentives and their other marketing strategy spending.
  
**Business Questions:**<br>
1. In general, does bidding on competitive keywords help our sales or damage competitors' sales?
2. In which regions/segments, does bidding on competitive keywords have the greatest negative impact on the competition’s sales?
3. For the regions/segments that bidding has a negative impact, which segments/regions should we focus?
4. For a particular region/segments, against which competitor do we have the greatest opportunity to impact sales negatively? 
3. Nationally, if sales for a particular one of Ford’s models are slumping, in which region do we see the greatest likelihood of successfully attacking our competitors?  Which competitor is the most vulnerable?  Which model (if not belonging to that competitor) is the most vulnerable? 

**Analysis Strategies:**<br>
1.Based on the following reasons: first, both our and competitors' sales varies from different segments, regions, and time periods, second, the spend on this month may have greater effect on next month or next two month's sales, I use the gap between our and competitors' next month (next two month) sales as dependent variable.
2.For the segment perspective, I separate the data into 14 different segments and try to find the "most fitted" model for each segment. From these different models, I can observe the impact of keyword bidding on the gap of sales. I assume the error terms for these models may correlate across each others so that seemingly unrelated regressions can be applied for this analysis. However, I don't have equal observations among the segments, the alternative plan is to run the ols first and random select equal observations for each segment, then use SUR to approach the models again. By comparing the coefficients of these two different regressions, there may be some interesting findings.
3.I do have equal amount of observations for each region, so I'll do the same approaches as segment part but using full data set instead.
