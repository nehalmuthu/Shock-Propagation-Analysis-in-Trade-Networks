# Shock-Propagation-Analysis-in-Trade-Networks

## Problem Statement:
Our objective is to observe and analyse how shocks propagate in a trade network and the factors causing its spread in the network. We first find the importance of a country in a network using centrality measures and MST , followed by its export import distributions(power law), and then find communities which are likely to get affected during a calamity (using community detection). Robustness Analysis is done to find out about the stability of the product  networks(crude oil and petroleum). 

## dataset :
[http://www.cepii.fr/DATA_DOWNLOAD/baci/doc/DescriptionBACI.html]
- Contains trade data from the year 2004 till 2018.

## Implementation Details:
- We start our analysis by finding:
    - Sub Shocks that affect individual agents
    - Sub connections between agents
    - Sub and the distribution of activity.  		
- Specifically, two models are applied to international trade data to explain relationships between exogenous shocks and fluctuations elsewhere in the network.
- The first model examines aggregate fluctuations at a country level by decomposing each country's imports of individual intermediate goods by whether or not each good has power-law-distributed exporter sizes, and whether or not the good is imported from a country with a large natural disaster. 
- The second model examines instead exogenous shocks that are not localized, but captured by the price of oil and its interaction with each country's role in the global trade network of all goods. 
- We analyse the importance of nodes by using degree and eigen centrality measures and  check for power-law distribution of exporters.
- Then we do robustness analysis to the crude oil and petroleum network. From that we observe that petroleum networks are more robust than crude oil networks. 
- Community detection algorithm is used to find the communities in the network so as to find the nodes which will be affected first during a calamity.
- To find the backbone structure of the network we use a weighted MST algorithm and represent the network. This will help us to find the crucial edges in the network.
- Finally we use the HITS algorithm to analyse the imports and exports of a country, which will help us to determine the market leaders in a particular product and also helps us to observe the trends of trading among countries.


