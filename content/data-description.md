---
title: Data 
prev: "/"
next: network-analysis
---

To delve into the intriguing world of beer reviews, we are leveraging the extensive Beer Advocate dataset. This dataset is derived from the beeradvocate forum and contains 1.5 million beer reviews starting from November 2011. Each review provides a score across five key qualities: appearance, aroma, palate, taste, and overall impression, along with a written text where the reviewer can elaborate on their oppinions and the qualities of the beer. Our analysis aims to decode what qualities of a beer people prefer, as well as identifying communities of people with different tastes in beers.

*An example from the data*
| beer/Name    | beerId | brewerId | ABV  | style      | appearance | aroma |
|--------------|--------|----------|------|------------|------------|-------|
| Sausa Weizen | 47986  | 10325    | 5.00 | Hefeweizen | 2.5        | 2     |

| palate  | taste | overall | time       | profileName | text             |
|---------|-------|---------|------------|-------------|------------------|
| 1.5     | 1.5   | 1.5     | 1234817823 | stcules     | A lot of foam... |


In order to manage our dataset more efficiently, we split the original dataset into two smaller sets: one containing the review scores and the other containing the review texts. After text lemmitization and compression, the used dataset is 203mb, with 1,560,428 samples and 13 features.

Due to the sheer size of the dataset, we narrowed our focus by trying to capture the more casual beer drinker. As such, we narrowed our scope down to users who have posted between 10 and 100 beer reviews, which should help us capture a broad yet relevant perspective on beer appreciation. 