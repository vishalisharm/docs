
## ASSIGNMENT 1
## ADVANCE ALGORITHMS LAB



### EXERCISE 1 

#### ASSUMPTIONS
- Undirected Graph (bidirectional)
- Duplicated edges are ignored when creating the edges list
- Unweighted Graph
- Used 1-based indexing (all the graphs vertices start from 1)

#### ALGORITHMS USED

1. Adjancey list: A 2d vector is maintained for the graph edges that stores two int values first one showing the
   u vertex and the second one showing the v vertex
2. Maximal Matching: An array is used to mantain the track of matched vertices to calculate the Maximal Matching.
3. Maximal Independent Set: Created an array of vertices and marked all the values as false, if a particular vertices
   is not false then include int the independent set and marked all the neighbours as true so that they can't be part of
   the set.

#### Time Complexity

1. For Adjacency List: First for loop runs E times to store hte edges and each iteration takes an input and push_back that
  input in the vector so that takes constant time and big oh(E) for the for loop so "O(E)" and then for printing the adjacency list
  the for loop iterates V(vertices) time which is "O(V)" so for the adjancey list part total time complexity become "O(V+E)".
2. For Maximal Matching: Here i initialize some attributes like matching etc for that constanct O(1) and then a for loop that iterates for
   E times so "O(E)", an array of size V(vertices) is made so "O(V)" then another for loop for the matching edges which runs M times but M<E
   so overall complexity of this part becomes "O(V+E)".
3. For Maximal Independent Set: Created an array of size V so O(V) then a for loop which traverses all vertices O(V), a nested for loop that iterates edges, so
   the final complexity of this part becomes "O(V+E)".
4. Total Time Complexity for algorithm - O(V+E).

#### MY INPUT - OUTPUT
![INPUT-OUTPUT](https://i.ibb.co/1tZsp9nF/Screenshot-2026-08-01-170918.png)
![INPUT-OUTPUT](https://i.ibb.co/pvJ2phPH/Screenshot-2026-08-01-180056.png)
### EXERCISE 2 

#### ASSUMPTIONS

- Undirected Graph (bidirectional)
- Duplicated edges are ignored when creating the edges list
- Unweighted Graph
- Used 1-based indexing (all the graphs vertices start from 1)

#### ALGORITHM USED

1. Adjancey list: A 2d vector is maintained for the graph edges that stores two int values first one showing the
   u vertex and the second one showing the v vertex
2. Line Graphh: After considering all the edges of graph as vertices the line graph is completed and then edge matching
   helps in finding the edges.
3. Maximal Independent Set: Created a boolean array to traverse every vertex of the line graph, adding it to the independent set and blocking its neighbour
   vertices.
4. The Maximal Independent set of the Line graph is the Maximal Matching of the original graph.


#### Time Complexity

- Taking input for edges: The for loop iterates E(edges) times and another operation takes constant time so O(E).
  Another loop iterates for V times for construction of edge list so O(V), overall for this part O(V+E).
- Vertices of line graph: Taking the edges of original graph as vertices for the line graph i run a for loop that
  iterates E times so O(E).
- Edges of line graph: There is a nested loop, the outer loop executes E times and the inner loop exutes E-i-1 times
  which is close to E so the time complexity become O(E2)​ and another loop runs for El times which is the edges of
  line graph so time complexity for this part becomes O(Esquare + El).
- Adjacency List: A for loop executed for edges.size() time which is E so O(E).
- Maximal Independent Set: For initialization of the array it take O(E), outer loop iterates E times and the inner loop
  iterates E X EL times so O(Ecube) as EL = O(Esquare).
- Total time complexity of the algorithm: O(E cube).

  #### MY INPUT-OUTPUT
  ![INPUT-OUTPUT](https://i.ibb.co/jvWDdN44/Screenshot-2026-08-01-175148.png)
  ![INPUT-OUTPUT](https://i.ibb.co/TNg1K74/Screenshot-2026-08-01-180258.png)
  ![INPUT-OUTPUT](https://i.ibb.co/VpLzPznG/Screenshot-2026-08-01-180305.png)

 
     
