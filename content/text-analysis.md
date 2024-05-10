---
title: Text analysis
prev: network-analysis
---

# Textual Analysis of Beer Reviews

## **Introduction:**
In our social science project, we embarked on a textual analysis of beer reviews to explore patterns of community formation based on preferences in beer consumption. Through this analysis, we aimed to understand the underlying characteristics and sentiments associated with different beer choices within distinct communities.

## **Community Identification:**
Upon analyzing the beer reviews, we identified three distinct communities based on commonalities in beer preferences and review sentiments. These communities were delineated based on shared characteristics observed in the reviews.

## **Methodology:**
The textual analysis was carried out by:

1. **Community Segmentation:** From the network graph, people were categorized into communities based on similarities in their beer reviews.
  
2. **Word Cloud Generation:** Word clouds were generated for the top-reviewed beers within each community, considering only those with more than 10 reviews and an overall score equal to or above 4/5. These word clouds visually represented the most frequently occurring adjectives in the reviews.

3. **TF-IDF and Exclusion:** The word clouds were constructed using TF-IDF (Term Frequency-Inverse Document Frequency) on lemmatized reviews, focusing solely on adjectives. Certain words were qualitatively excluded if they were deemed irrelevant to offering insights about the beer.


## **Analysis by Community:**

### **Community 1:**
![Community 1 Word Cloud](/images/community0.png)
- *Beer Choices:* Quad, American Double/Imperial IPA, Flander Oud Bruin.
- *Top Words in Word Clouds:* Dark, brown, sweet, light, deep, golden, orange, crisp, sweet, fresh, light, white, fresh, soft, yellow.
- *Interpretation:* Community 1 appears to favor a diverse range of beer styles, including both darker and lighter options. The descriptive terms suggest an appreciation for nuanced flavors, colors and varied sensory experiences.

### **Community 2:**
![Community 2 Word Cloud](/images/community1.png)
- *Beer Choices:* Old Ale, American Double/Imperial Stout.
- *Top Words in Word Clouds:* Dark, deep, aging, smooth, level, caramel black, dark, sweet, vanilla, carbonated.
- *Interpretation:* Community 2 exhibits a preference for robust and full-bodied beers, characterized by rich, deep flavors and smooth textures. The descriptive terms imply a fondness for complexity and depth in beer profiles.

### **Community 3:**
![Community 3 Word Cloud](/images/community2.png)
- *Beer Choices:* American IPA, American Double/Imperial IPA, American Strong Ale.
- *Top Words in Word Clouds:* Golden, smooth, crisp, easy, bitter, floral, orange, smooth, intense, easy.
- *Interpretation:* Community 3 exhibits a preference for aromatic beers, with a focus on bold flavors and refreshing characteristics as IPAs are known for. The word choices suggest an inclination towards beers that offer a balance between bitterness and smoothness, with vibrant fruity and floral notes.

## **All beers in the communites:**
Taking a look at the wordclouds for all reviews of well liked beers within a community (score ≥ 4/5), we see the communities as a whole exhibit similar preferences to eachother, however a slight preference skew is still present, similar to what was found between the top beers

![Community 3 Word Cloud](/images/community2.png)
### Top TF-IDF over communities (from left to right)
- Community 1: light, sweet, dark, smooth, brown
- Community 2: dark, sweet, light, smooth, brown
- Community 3: sweet, light, dark, smooth, white

Upon examining the word clouds representing all reviews of well-liked beers within each community (with a score ≥ 4/5), it becomes evident that while the communities have slightly different preferences for their top beers, a consistency exists between the preferences in all beers. For instance, descriptors like "sweet" and "smooth" emerge prominently across all communities, suggesting a collective preference for beers with these attributes.


## **Conclusion:**
The beer choices within each community provide insights into the distinct preferences and sensibilities of the individuals comprising them. **Community 1** exhibits a wide range of beer styles, including both darker and lighter options, suggesting an appreciation for nuanced flavors and varied sensory experiences. **Community 2** demonstrates a preference for robust and full-bodied beers, characterized by rich, deep flavors and smooth textures, indicating a fondness for complexity and depth in beer profiles. **Community 3** exhibits a preference for fresh and aromatic beers like IPAs, with a focus on bold flavors and refreshing characteristics, suggesting an preference for beers that offer a balance between bitterness and smoothness, with vibrant fruity and floral notes.

Upon examining the word clouds representing all reviews of well-liked beers within each community, it becomes evident that while the communities have slightly different preferences for their top beers, a consistency exists between the preferences in all beers. For instance, descriptors like "sweet" and "smooth" emerge prominently across all communities, suggesting a collective preference for beers with these attributes.

## **Final thoughts and points of contention:**
Due to memory limitations, the analysis is carried out on a subset of the data instead of the full dataset. We tried to narrow down the scope by limiting it to users with between 10 and 100 reviews in hopes of capturing the more casual drinker. As such, the presented data will not necessarily be indicative of the full dataset, and the communities will likely look very different.

The generation of these wordclouds rely on review scores, which for people can be highly subjective. Some people may be more inclined to score the beer higher or lower despite having the same oppinion about it, for example a beer rated 3/5 should in theory be average, howeever due to a leniency bias, some people might rate a beer they percieve as average higher.

The analysis does not consider demographic factors such as age, gender, or geographic location, which could influence beer preferences. Without this information, the findings may not be generalizable to broader populations or demographics. In the wordclouds, we see American beers featured prominently, which may indicate that the majority of the reviewers are American. The beeradvocate forum is in english also, this gates people who don't speak english to review beers, which introduces a bias.
