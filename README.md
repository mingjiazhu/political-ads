# political-ads

In this project, I worked on data analysis and prediction based on snapchat Political Ads dataset.

## Introduction

The datasets contains data of political ads that have been served on Snapchat’s Advertising platform in 2018 and 2019. The datasets of both years contain 34 columns, which include comprehensive infomation about political ads, such as spend, start and end date, organization name, advertiser name, and candidate ballot information.

In this project, I answer the following questions:
What are the most prevalent organizations, advertisers, and ballot candidates in the data?
Are there any of them could be recognized?

In order to answer these questions, I search through the datasets to find out related information. I notice that the datasets contain Impressions, OrganizationName, PayingAdvertiserName, and CandidateBallotInformation columns. From the data in these columns, I could figure out the most prevalent organization, advertiser, and ballot candidate based on the statistics about impressions. The reason why I utilize impressions to evaluate whether organization, advertiser, and ballot candidate are prevalent is that impressions represent how often the ads are shown. This quantifies the popularity of the ads, so that I could know the prevalence of ads from this information.

Then I focus on prediction problem. At here, I try to predict how much was spent on an advertisement. I would like to utilize different features in the dataframe such as Impressions, OrganizationName, and PayingAdvertiserName. By combining these different features, I would like to build regression models in the project, so the problem is regression problem. The target variable is Spend. I try to utilize different features in the dataframe to predict the spend of advertisements. For the baseline model, I consider the spend might be related to Impressions, OrganizationName, and PayingAdvertiserName. In the final model, I add more information by engineering features such as StartDate and CountryCode.

Our evaluation metric that is used for two models is mean absolute error. It could help me to clearly see the differences between predictions and actual values. By comparing the mean absolute errors of different models, I could figure out the best model which generates the perdictions that are closest to actual values.


