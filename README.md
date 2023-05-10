# dijkstra-s-algorithm
In this project,  Dijiktra’s algorithm is used to find the shortest path between two vertices in a G set. The code was run three times with three different source vertices and destination vertices to display the results.

For more information about me, please visit my LinkedIn:

[![LinkedIn][LinkedIn.js]][LinkedIn-url]

<!-- ABOUT THE PROJECT -->

## About The Project:

### Backgroud Terminology: 

It's important to have a good idea about Dijkstra's to understand the terminology used throughout this project.

Please visit the following links for a more detailed explanation of the concept:

[https://www.spiceworks.com/tech/artificial-intelligence/articles/what-is-linear-regression/#:~:text=Linear%20regression%20is%20an%20algorithm,machine%20learning%20for%20predictive%20analysis.
](https://www.geeksforgeeks.org/dijkstras-shortest-path-algorithm-greedy-algo-7/)

### Introduction:

The aim of this paper is to implement Dijiktra’s algorithm on a G1 set to find the shortest
paths in the graph. A function that prints the least cost path from the source to the destination
node was developed, named printLeastCostPath(). The results of three source nodes to their
destination nodes were displayed as an example:
- Source vertex 1 to destination vertex 107 had a total path cost of 107
- Source vertex 1 to destination vertex 101 had a total cost path of 101.
- Source vertex 5 to destination vertex 80 had a total path cost of 144.
the subpaths and their cost to the destination nodes (107, 101, 80) were also displayed.
The time complexity of this algorithm is O(V2
), where V is the number of vertices in the graph.
As for the space complexity, it is also O(V2
) because a 2d matrix representation of the matrix
was used, with its data populated from the input file downloaded from the Gset standard set of
graphs used for testing and comparison of various algorithms.


### Dataset:

Data used in this paper is the standard set of graphs “G-set” that is often used for testing
and comparison of various algorithms. These G sets could be accessed using the Stanford
libraries. The set picked in this paper is the G1 set, which has 800 vertices and 19716 edges, as
shown on the top row in figure 2.
The weights that came in the files were all 1; the third column was edited into a list of
randomly generated weights. This was done by running a python script which read the file and
copied it to a new one replacing the 1 with a random number.

![image](https://github.com/SaliElloh/dijkstra-s-algorithm/assets/112829375/dc3c4612-64d2-4081-92d4-ac060fce7c4b)
Figure 1: Vertex one and all the vertices connected to it are shown in the first and second
column, respectively. The third column is the “weight” or the cost to get between vertex one (in
this example) and the connecting vertices


### :



### PseudoCode used:

In this section, I'll delve deep into the psuedocode used throughout this project. This will help you understand the general structure of the code prior to running it.

1) Mark all vertices as unvisited, then create the unvisited set, which is a collection of all
undiscovered nodes.
2) Assign a tentative distance value to each node: Mark all nodes with an infinity distance at
first, except the source node, which is marked with a zero distance. Because no path is
known between any other vertex aside from the source, all tentative distances have been
originally set to infinity.
3) Consider all of your current node V's univisited neighbors U.
4) We update the cost[U] + weight of UV if it counts a lower cost than the existing cost[v].
5) We mark the code as visited and remove it from the unvisited collection once we have
finished taking into account all of the unvisited neighbors of this particular node. There
will be no further visit to this node [3].
6) if the destination has been checked off as visited or if the shortest distance between nodes
in the unvisited set is infinite, then the algorithm is then stopped. There is no
connection between the node and the other nodes that haven't been visited.
7) As an alternative, we can choose the unvisited node marked with the least tentative
distance, set it as the new current node, and then repeat these steps U–V times, or until all
the vertices have been visited.[3]

## Getting Started:

To get the project running, there's a couple of programs and steps needed.

### Built With:
The frameworks and libraries used within this project are:
* [![Scikit-learn][scikit-learn.js]][scikit-learn-url]
* [![TensorFlow][Tensorflow.js]][Tensorflow-url]
* [![NumPy][NumPy.js]][NumPy-url]
* [![Matplotlib][Matplotlib.js]][Matplotlib-url]

### Prerequisites:

1. Python: PyCharm is an IDE for Python development. 
2. PyCharm:  you can download Pycahrm from JetBrains website.
3. Operating system: PyCharm is available for Windows, macOS, and Linux. 
4. Hardware requirements: PyCharm has minimum hardware requirements, including a multi-core processor, at least 4 GB of RAM, and a minimum screen resolution of 1024x768.
5. Tensorflow, Scikit-learn, NumPy, Matplotlib installed on your computer

### Steps to run the code:

1. Download the “model-selection-via-cross-validation” zip file. 

To do that, simply press on the zip file, then press "view raw" as shown below to download it:

![image](https://github.com/SaliElloh/model-selection-via-cross-validation/assets/112829375/2412942f-c491-4f77-865c-7c7ae27c8a22)

All the files inside that zip files are uploaded seperately as well.

3. Extract all files found in the zip file:

    In the file, you’ll find 6 files, titled:

     a. CVfor0to12:  performs the k fold cv using the given training data to select the optimal
degree.
      b. Optimal Degree_trained: after finding d*, perform linear regression for  all the data using the optimal degree found: finds the polynomial coefficients, and fit
      
      c. CVfor12Only: performs k fold cv to select the optimal regularizer value, λ*
      
      d. Optimal alpha_trained: performs ridge regression for λ* selected using all the data
      
      e. Test.csv: contains all the test data used in the project
      
      f. Train.csv: contains all the training data used in the project
      
3. Run each file separately to get the final results of the project


## Results: 
the results of this project include: 

Three different source and destination vertices were used to test the results using this
code. As shown in table 1, when the source vertex 1 and the destination node 150 were inputted,
the program outputted the distance cost of each subpath, and the cost of the total path. The same
is done for source vertex 1 and destination vertex 101, and lastly source vertex 5 and destination
vertex 80. For more details about the code, please refer to the attached file containing the code,
where a step by step outline for the code is shown



<!-- LICENSE -->
## License:

No License used.

<!-- CONTACT -->
## Contact:

Sali E-loh - [@Sali El-loh](https://www.linkedin.com/in/salielloh12/) - ellohsali@gmail.com

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments:

* Special thanks to Professor Luis Ortiz at the University of Michigan - Dearborn for assigning and helping with this project in his Computational Learning class.

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[LinkedIn.js]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
[LinkedIn-url]: https://www.linkedin.com/in/salielloh12/
[Tensorflow.js]: https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white
[Tensorflow-url]: https://www.tensorflow.org/
[NumPy.js]: https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white
[NumPy-url]: https://numpy.org/
[Matplotlib.js]: https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black
[Matplotlib-url]: https://matplotlib.org/
[scikit-learn.js]: https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white
[scikit-learn-url]:https://scikit-learn.org/






