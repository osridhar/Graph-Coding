# Graph-Coding
## Example Usage

```python
import networkx as nx
from graph_operator import GraphOperator

# Create a graph
graph = nx.Graph()
graph.add_edges_from([(1, 2), (1, 3), (2, 3), (2, 4), (3, 4)])

# Create a GraphOperator instance
graph_operator = GraphOperator(graph)

# Calculate the average degree
average_degree = graph_operator.average_degree()
print(f"Average degree: {average_degree}")

# Find the vertex with the highest degree
vertex_with_highest_degree = graph_operator.vertex_with_highest_degree()
print(f"Vertex with highest degree: {vertex_with_highest_degree}")

# Determine the number of connected components
connected_components_count = graph_operator.connected_components_count()
print(f"Connected components count: {connected_components_count}")

# Calculate the open/closed triangle ratio
open_closed_triangle_ratio = graph_operator.open_closed_triangle_ratio()
print(f"Open/closed triangle ratio: {open_closed_triangle_ratio}")

# Find the closest node with interest
closest_node_with_interest = graph_operator.closest_node_with_interest(1)
print(f"Closest node with interest: {closest_node_with_interest}")

# Find the person with the highest interest
person_with_highest_interest = graph_operator.person_with_highest_interest(1)
print(f"Person with highest interest: {person_with_highest_interest}")

# Calculate the smallest ratio of hobby graph distance
smallest_ratio_hobby_graph_distance = graph_operator.smallest_ratio_hobby_graph_distance()
print(f"Smallest ratio of hobby graph distance: {smallest_ratio_hobby_graph_distance}")
