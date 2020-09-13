# Chocolate Data Exploration
## by Abbie Weisenbloom

## Exploratory Notebook uses one graph with Networkx

I tried to use a network graph in one plot that requires the Networkx.  If this is a problem, I can resubmit! If you want to run the graph, please install it if you don't have it already or you can just skip the cell : https://networkx.github.io/documentation/stable/install.html . 

## Dataset

This document explores a kaggle dataset - Chocolate Bar 2020. You can find it [here](https://www.kaggle.com/soroushghaderi/chocolate-bar-2020).  There are 2224 chocolate bars in the dataset with 20 features (rating, company, company_location, review_date,country_of_bean_origin, specific_bean_origin_or_bar_name, cocoa_percent, counts_of_ingredients, beans,cocoa_butter, vanilla, lecithin, salt, sugar, sweetener_without_sugar, first_taste, second_taste, third_taste,fourth_taste).  It took me awhile to orient myself with all of the ways to explore this data, so I focused on the chocolate bar tastes, ingredients, and bean of origin.

All of the chocolate bars in this dataset are 55% cocoa and above, which means they are various intensities of dark chocolate.
4.0 - 5.0 = Outstanding<br>
3.5 - 3.9 = Highly Recommended<br>
3.0 - 3.49 = Recommended<br>
2.0 - 2.9 = Disappointing<br>
1.0 - 1.9 = Unpleasant<br>

## Summary of Findings

Since there were so many variables and I wasn't sure until the end of the exploration which ones would actually work for the presentation. I explored many possible relationships.  I quickly found that many of the variables were unique categorical ones and were too numerous to plot so I had to get creative with how many and which ones I chose to focus on.  I decided that the Top 20 of any given categorical variable could be managed.  To do this I calculated relationships based on the mean ratings of categories. 

I started by exploring individual distributions for rating rating_categories to see if how the bars were rated overall. Most of them were recommended to highly recommended. I also plotted the ingredients which showed that out of 6 possible ingredients, there were only 3 or 4 major ones - beans & sugar. The beans obviously play largely into flavor rating so I plotted the relationship of bean of origin to average rating. 

I also focused on the 3 tastes since they are really fascinating and descriptive.   I plotted based on rating categories as well as these groups to see how they correlated with the ratings.


I used bar plots to plot the first, second, and third tastes since they were the clearest way to view the data. I used different colors to make them stand out. 

In addition to the ingredients and tastes, I also attempted to plot the country of bean origin with the unique company names. I found this challenging and experimented with a Networkx graph to plot relationships since there were so many. This was too difficult to interpret to put in the presentation but I'd like to learn about and explore network graphs more.

## Key Insights for Presentation

For this presentation I focused on what flavor and ingredient characteristics are correlated with the chocolate ratings provided in the dataset. I started by showing the rating system - numeric and categorical.  Then I showed the distribution of ingredients as well as which ones were associated with the highest rated chocolate. I also showed the distribution of the first, second, and third tastes which is interesting to see because there are so many of them and they are very descriptive and evocative. Since there are so many, I only plotted the top 20. Next,I plotted them against all of the categories to show how the tastes correlated with the categories.  

Since the country of bean origin is the main ingredient used in the chocolate, I plotted its relationship to the ratings as well.