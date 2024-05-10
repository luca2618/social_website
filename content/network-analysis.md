---
title: Network analysis
prev: data-description
next: text-analysis
---

## **Constructing the Network**
The network we created from dataset, consisted of 2 types of nodes. Person nodes and beer nodes, each interlinked by a person review of a beer. Ultimately we were interessted in communities of beer drinkers, and therefore projected the network onto the people nodes. Furthermore we weighted each edge between 2 people with the sum of an agreement score for each beer they shared.

## **Network properties**
The network end up being completely connected, meaning that there are no isolated nodes of people drinking beers that no other person


## **Weight analysis**

![Graph weight distribution](/images/weight.png)

## **Degree analysis**
To better investigate the degree properties of the network we made a random comparison network with the same amount of nodes and same probability of an edge between nodes. As seen in the graph the structure of the network is far from similar to that of a random network. It significantly more spread, consisting of more high and low degree nodes, corresponding to people with more/less reviews or more/less popular beers in their reviews. Showing that there is wider range of beers drinkers than from a random network where people are equally likely to review and for a beer to be reviewed. This aligns with our expectation of the dataset representing a wider range of beers drinkers and range popularity beer. 
![Graph degree distribution](/images/degree.png)
### **Assortivity**
The assortivity being slightly negative indicates that 
