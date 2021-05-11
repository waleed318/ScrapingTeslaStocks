# ScrapingTeslaStocks
## Problem
### I am interested in buying a tesla but i would like to perform some market research first.
### I know that any new technology has issues at first which are settled overtime.
### So, I found a website: https://www.bloomberg.com/graphics/2019-tesla-model-3-survey/
### which has a barplot/histogram that shows minor issues and major issues reported overtime
### before making a decision i wanted to scrape the data load it into a pandas dataframe and plot a curve for minor against major issues (Because i dont like histograms)
### But when i tried to scrape the data i found out that the values that i am trying to scrape 
### (e.g Minor Issues = 63.7,Major Issues = 10.0 for Jan 2018 and so on) are being generated dynamically i.e. by javascript and i am not able to see those values in html.
![TeslaStocksOnBlombergSite](https://user-images.githubusercontent.com/68495234/117834003-405fff80-b290-11eb-86d6-6563f1647015.JPG)

## Solution
### 1. Extracted Data From Bloomberg site using selenium
###  a.Data only visible when we hover mouse over it.
###  b.I found out that data became visible when we hover mouse over a div tag names "rect".
### 2. Store Data in the form of Pandas DataFrame.
### 3.Visualized with seaborn library
