# Effects of the Borrowers Interest Rates on loans
## Dataset
I used [prosper.com's](http://www.prosper.com/) gathered data about loan borrowers, there are 113937 listings in the pulled data ranging from 2006 till early 2014. Prosper is an investment company located in California, USA.

The dataset can be found in my [githubrepo](https://github.com/islamellawendy/Communicate-Data-Findings/blob/master/prosperLoanData.csv). While this [link](http://ggplot2.tidyverse.org/reference/diamonds.html) provides the dictionary of definitions to the variables in the dataset.
## Summary of Findings
In my exploration, I started by first identifying some interesting information about the borrowers, the salary range distribution, their employment status and the years of experience of these borrowers, also how many are home owners playes a part in the first 2 aspects since slightly less than half of the borrowers do not own a home. Revisiting in my exploration the employment status I wanted to see this in effect with the interest rates, with the highest rates were given to the unemployed bunch of borrowers.

Also it was insightful to see the other side of the story, the investors. [The Estimated Effective yield](https://www.investopedia.com/terms/e/effectiveyield.asp) provides the return rate on investing in loans, first by seeing the distribution then by seeing the credit grade.

My core was always looking at the interest rates (Borrower rate and Borrower APR) and their interactions with other variables, as said I first studied the numeric variables in my dataset in reaction. A strong positive correlation with the estimated effective yield and another strong negative with the prosper score (more on the correlations in the slide deck).

Also, I was exploring the listing category in order to see the average rates per purpose of the loan. Zooming in on this I found that the majority of borrowers take loans for Debt Consolidation. I zoomed in on this category to understand more.

Finally, I looked at the interest rates' trend over time, with the same look out on the two the loan amounts and the prosper score.
## Key insights and takeouts
### Insights
In my representation of data, I am using simple yet very descriptive visualizations, for univariate plots it is either a histogram or a bar plot. As for the bivariate plot I am using various plot schemas, with the box plot as the most complex of all. 

Please note that the time series uses a moving average of 3 periods in order to eleminate the effect of the missing data found in the economic crisis era.

Finally, for the multivariate I am using a heatmap for the correlation plot and a scatter plot with encoded color bar for the zoom in I did on the Debt Consolidation category's data.
Some advanced studies can be done on this analysis if we bring in more variables from the source data. However, I have no Financial background and my study is based on my observations on the various behaviours I get.
### Takeouts
One point I do not affirm my understanding about is the Debt to income ratio in the multivariate analysis I did on the Debt Consolidation listing, I cannot confirm or dismiss that a debt to income ratio as high as 10 is actual (you have 10 times a debt than your income!).

**N.B.:** Please use `jupyter nbconvert slide_deck_template.ipynb --to slides --post serve --template output-toggle.tpl` for initializing the slide deck presentation in the command terminal.