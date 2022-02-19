# Friend suggestion system for social networks
## MIC Algorithm

Social Network is a big graph with nodes being people and edges being relationships. This could be undirected like facebook or directed as in case of Twitter (Follower - Followee relationship).

Accepting friend suggestions would add new edges in the network. There are various factors by which we can add edges. Some factors are mutual friendships, ie. People with more common friends are more likely to become friends in the future. Similarly, the same geographical location, language, workplace etc. are other factors where friendships are most probable. Communities with common interests like music, sports or movies have higher density of friendship relationships among them.

The factors like Mutual Friends, similar interests, closeness in graph are used to suggest friends to users. The proposed algorithm is **MIC (Mutual Friends, Interests, Closeness) Algorithm**.

<p align="center">
    <img width="60%" alt="MIC Algorithm" src="https://user-images.githubusercontent.com/53406309/154812848-ba155624-6adf-4179-94e9-5dcac207aa34.png">
</p>

---

## Friend Suggestion - Dataset
- Collected from real world by circulating *google forms* to classmates, friends, etc.
- The following fields were included in the form:
    - Roll No & Name
    - City/District
    - Languages Known
    - Interests
    - List of Close Friends
- This dataset contains the details of 60+ students. [Click Here to view the Dataset](./Data/Friend%20Suggestion.csv)

----

## Algorithm and Steps
1. Importing libraries and loading data from csv into python
2. Preprocessing steps
    - Preprocess node list (Students as Nodes)
    - Helper functions 
        - Roll number -> Name Conversion
        - Roll number -> Node number Conversion
        - Node number -> Roll number Conversion
    - Preprocess edge list
    - Preprocess interests and languages from the survey data.
3. Networkx representation of graph.
4. Visualisation in networkx.
5. **MIC ALGORITHM**
    - Iterate through 2 to k levels of BFS:
      - Score based on similarities of location, interests, language is calculated.
      - The score is augmented if number of mutual friends is high.
      - The score is multiplied by the weight of the level. (Closer levels have higher weight)
      - The final scores are sorted in descending order and friends are suggested accordingly.
6. Suggest friends for everyone.
7. Accuracy Test Metric
    - Remove a certain percentage of the edges.
    - Make this as the test graph.
    - Run the Friend Suggestion Algorithm.
    - Finally check the accuracy by comparing with the original graph.
8. Gephi color coded visualisation of BFS and suggestions.
9. Future scope
    - Sparse graph due to data can be made dense.
    - Extension to between departments and for other departments of the college. 

---

## Images

### Visualisation in Gephi
- Gephi color code : 
    - **Level 1 (friends already)** - Red
    - **Level 2** - Green 
    - **Level 3** - Yellow 
    - **Level 4**- Blue
    - **Suggested Friends** - Violet

<p align="center">
    <img width="60%" alt="Gephi" src="https://user-images.githubusercontent.com/43994542/154804779-b5b310ca-efb1-45ab-b0ac-ecc8f4caafc4.png">
</p>

### Visualisation in networkx

![Networkx](https://user-images.githubusercontent.com/43994542/154804475-d6314c76-ba48-40d1-a1ee-ebb12e4ba83a.png)

---

## Reference links

- [Link Prediction in Social Networks](https://medium.com/@gorerohan15/link-prediction-in-social-networks-599e6d9bed9b)
- [A Guide to Link Prediction – How to Predict your Future Connections on Facebook](https://www.analyticsvidhya.com/blog/2020/01/link-prediction-how-to-predict-your-future-connections-on-facebook/)

---

## Note
This project is done by a team of 5 students as a part of Artificial Intelligence Lab.
