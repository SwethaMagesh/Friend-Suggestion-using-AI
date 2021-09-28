# Friend suggestion system for social networks

Social Network is a big graph with nodes being people and edges being relationships. This could be undirected like facebook or directed as in case of Twitter (Follower - Followee relationship).

Accepting friend suggestions would add new edges in the network. There are various factors by which we can add edges. Some factors are mutual friendships, ie. People with more common friends are more likely to become friends in the future. Similarly, the same geographical location, language, workplace etc. are other factors where friendships are most probable. Communities with common interests like music, sports or movies have higher density of friendship relationships among them.

The factors could be built into a likelihood function and a search algorithm could be implemented to find nodes which maximise this function from a specific node. Combination of algorithms like BFS, shortest path etc. can be used to suggest friends to users.

[Link to colab](https://colab.research.google.com/drive/1IOgQiJRKYY_BjmmTMtFuqAFrSNwXShP8?usp=sharing)

## Interesting links

- [Medium Article 1](https://medium.com/@gorerohan15/link-prediction-in-social-networks-599e6d9bed9b)
