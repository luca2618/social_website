---
title: Network analysis
prev: data-description
next: text-analysis
---

## **Constructing the Network**
The network we created from dataset, consisted of 2 types of nodes. Person nodes and beer nodes, each interlinked by a person review of a beer. Ultimately we were interessted in communities of beer drinkers, and therefore projected the network onto the people nodes. Furthermore we weighted each edge between 2 people with the sum of an agreement score for each beer they shared.

## **Network properties**
The network end up being completely connected, meaning that there are no distinc sets of people driking only distincs sets of beers. The dataset has many reviews, so its expected that for any beer that has been reviewed that there is at least one other person that has reviewed that has tried another beer. 


## **Weight analysis**
The weight of the edges mainly show that there are very few connection that are considered negative, that 2 people disagree on the beers they drink. This is mostly expected, as we expect most people to drink and review the beers that they like and therefore mostly agree. Furthermore, if a beers is bad we likewise would expect people to aggree on them. The negative scores do however represent an important demografic of the edges in the network, as they represent disaggrence on beers, meaning distinct differences in the perception of a beer or several beers. That there are negative weights at all therefore shows us that there are people in the network that mainly disagree on the beers that they drink, and they therefore likely have distint different tastes. Its not essential to showing that there exist different communities of beer drinkers, but is interesting as they show the existence of people trying out different beers and having mixed opinions on them.
![Graph weight distribution](/images/weight.png)

## **Degree analysis**
To better investigate the degree properties of the network we made a random comparison network with the same amount of nodes and same probability of an edge between nodes. As seen in the graph the structure of the network is far from similar to that of a random network. It significantly more spread, consisting of more high and low degree nodes, corresponding to people with more/less reviews or more/less popular beers in their reviews. Showing that there is wider range of beers drinkers than from a random network where people are equally likely to review and for a beer to be reviewed. This aligns with our expectation of the dataset representing a wider range of beers drinkers and range popularity beer. 
![Graph degree distribution](/images/degree.png)
### **Assortivity: -0.1045**
As the coefficient is around zero, it suggests a random mixing pattern of degree. However, it still negative, which show that high degree node are slightly more likely to connect to low degree node (users who share reviews with fewer users). This could suggest that people who have only reviewed fewer or less popular beer are more likely to have at least one beer in common with a person who has more reviews / reviews of more popular beers, which makes sense.
