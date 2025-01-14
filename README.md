# Social Network Analysis of Hashtag Co-occurrence

## **Project Overview**
This project analyzes a social network of hashtags derived from user-generated posts across multiple platforms. The primary goal is to construct and analyze the network, compare it with theoretical models, and address the research question:
> *"Which hashtags are most central and influential in the network, and how do they contribute to its fragmentation?"*

---

## **Dataset Description**
The dataset contains the following attributes:
- **Text**: Content of user posts.
- **Hashtags**: Keywords/topics marked with `#`.
- **Platform**: Source platform (e.g., Twitter, Instagram).
- **Engagement Metrics**: Likes, retweets, and other interaction data.
- **Timestamps**: Date and time of posts.

**Preprocessing Steps**:
1. Extracted hashtags from posts.
2. Removed entries without hashtags.
3. Parsed hashtags into a structured format for network construction.

---

## **Network Construction**
The social network was constructed as follows:
- **Nodes**: Unique hashtags.
- **Edges**: Co-occurrence of hashtags within the same post.
- **Edge Weights**: Frequency of co-occurrence.

**Key Network Statistics**:
- Nodes: 975
- Edges: 692
- Density: 0.001457
- Connected Components: 284

---

## **Network Analysis**
1. **Degree Distribution**:
   - Average degree: 1.419.
   - Indicates moderate connectivity among hashtags.

2. **Clustering Coefficient**:
   - Average clustering coefficient: 0.0.
   - Shows no significant tendency for hashtags to form tightly knit groups.

3. **Connected Components**:
   - Total: 284 components.
   - Largest component: 15 nodes.

4. **Path Analysis**:
   - Average path length: 8.13.
   - Diameter (largest component): 19.

5. **Centrality Measures**:
   - Top hashtags: `#Serenity`, `#Excitement`, `#Gratitude`.
   - Metrics include degree, betweenness, and closeness centrality.

---

## **Comparative Analysis**
The actual network was compared with theoretical models:
- **Erdős–Rényi (ER)**:
  - Similar density and fragmentation.
- **Barabási–Albert (BA)**:
  - Higher average degree, single connected component.
- **Watts–Strogatz (WS)**:
  - Small-world properties with a single connected component.

---

## **Research Question**
**"Which hashtags are most central and influential in the network, and how do they contribute to its fragmentation?"**

**Findings**:
- Central hashtags (e.g., `#Serenity`) are influential but primarily active in isolated clusters.
- Fragmentation arises due to limited bridging between communities.
- Recommendations include promoting bridging hashtags to reduce fragmentation.

---

## **Conclusion**
This project provides insights into the structure and dynamics of hashtag networks, highlighting areas for improvement in connectivity and community bridging. Future work can explore dynamic trends and external factors influencing hashtag co-occurrence.

---

## **Repository Structure**
- `data/`: Contains the processed dataset.
- `notebooks/`: Jupyter notebooks with code for preprocessing, network analysis, and visualization.
- `results/`: Visualizations, statistics, and comparison tables.
- `README.md`: Project overview and instructions.

---

## **How to Run the Project**
1. Clone the repository:
   ```bash
   git clone https://github.com/erenbg1/B107-Data-Driven-Strategic-Decision-Making.git
