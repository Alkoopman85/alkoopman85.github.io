## SQLite Database of the Yelp Dataset

**Project description:** This project focussed primarily on implementing and populating the database with the yelp dataset. It contains users, reviews, busisness, tips, checkins, and photos. These tables and their relationships were examined, and a networkx graph was build baed on the user friend groups.<br>
[YelpDataBase Class](https://github.com/Alkoopman85/Yelp_sqlite_database/blob/main/database.py) | [Database Inspection](https://github.com/Alkoopman85/Yelp_sqlite_database/blob/main/quick_inspection.ipynb)

---
### Figure 1: Entity Relationship Diagram

<img src="images/entity_relationship_diagram.png?raw=true"/>

---
### Figure 2: Friend Graph Degree Histohram
This plot shows up to degree 40. However the maximum degree is 6869 in the graph. This was done for the sake of visualizing the drgree distribution.
<img src="images/graph_degree_dist.png?raw=true"/>

---