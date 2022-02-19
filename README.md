# Friend suggestion system for social networks

Social Network is a big graph with nodes being people and edges being relationships. This could be undirected like facebook or directed as in case of Twitter (Follower - Followee relationship).

Accepting friend suggestions would add new edges in the network. There are various factors by which we can add edges. Some factors are mutual friendships, ie. People with more common friends are more likely to become friends in the future. Similarly, the same geographical location, language, workplace etc. are other factors where friendships are most probable. Communities with common interests like music, sports or movies have higher density of friendship relationships among them.

The factors like Mutual Friends, similar interests, closeness in graph are used to suggest friends to users. The proposed algorithm is MIC (Mutual Friends, Interests, Closeness) Algorithm.


## Algorithm and steps
1. Importing libraries and loading data from csv into python
2. Preprocessing steps
    - Preprocess node list(students as nodes)
    - Helper functions (Roll no, node no and name interconversion)
    - Preprocess edge list(existing friend structure)
    - Preprocess interests and languages from the survey data. 
 3. Networkx representation of graph
 4. Visualisation in networkx
 5. MIC ALGORITHM
    - Mutual friends 
    - Interest
    - Location
    - Language
    - Final score 
 6. Suggest friends for all students
 7. Accuracy is tested
    - Remove some edges and check if they would be suggested
 8. Gephi color coded visualisation of BFS and suggestions
 9. Future scope
    - Sparse graph due to data can be made dense
    - Extension to between departments and for other departments of the college. 
    
    
 ## Images

 
 - Gephi color code : **Level 1 (friends already)** - red, **level 2** - green , **level 3** - yellow, **level 4**- blue, **suggested friends** - violet
 
 <img width="473" alt="image" src="https://user-images.githubusercontent.com/43994542/154804779-b5b310ca-efb1-45ab-b0ac-ecc8f4caafc4.png">
 
  - Visualisation in networkx
 ![image](https://user-images.githubusercontent.com/43994542/154804475-d6314c76-ba48-40d1-a1ee-ebb12e4ba83a.png)


[Link to colab](https://colab.research.google.com/drive/1oTWj-OM1v1SF1a-Oz3zjD7AVGrlH1UCH?authuser=1)

[DATA spreadsheet](https://docs.google.com/spreadsheets/d/1W7CVlwp7sqb9YnByTjMy6OHff8ceBl_ZxgF2aPvhc88/edit#gid=0)

## Reference links

- [Link Prediction in Social Networks](https://medium.com/@gorerohan15/link-prediction-in-social-networks-599e6d9bed9b)
- [A Guide to Link Prediction – How to Predict your Future Connections on Facebook](https://www.analyticsvidhya.com/blog/2020/01/link-prediction-how-to-predict-your-future-connections-on-facebook/)

## Note
This project is done by a team of 5 students as a part of Artificial Intelligence Lab.
