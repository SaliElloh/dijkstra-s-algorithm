# dijkstra-s-algorithm
This project implements Dijkstra's algorithm to find the shortest path between two vertices in a G set. 

For more information about me, please visit my LinkedIn:

[![LinkedIn][LinkedIn.js]][LinkedIn-url]

<!-- ABOUT THE PROJECT -->

## About The Project:

### Background Terminology: 

It's important to have a good idea about Dijkstra's to understand the terminology used throughout this project.

Please visit the following links for a more detailed explanation of the concept: <a href="https://www.geeksforgeeks.org/dijkstras-shortest-path-algorithm-greedy-algo-7/" style="display:inline-block;background-color:#8a8a8a;color:#fff;font-size:16px;padding:10px;border-radius:5px;text-decoration:none;">Dijkstra's Algorithm</a>

### Introduction:

The objective of this project is to apply Dijkstra's algorithm on a G1 set to determine the shortest paths in the graph. A new function called "printLeastCostPath()" was developed to print the path with the least cost from the source node to the destination node. The code was executed three times with different source and destination vertices to demonstrate the results.

These three source nodes are: 
- Source vertex 1 to destination vertex 107 had a total path cost of 107.
- Source vertex 1 to destination vertex 101 had a total cost path of 101.
- Source vertex 5 to destination vertex 80 had a total path cost of 144.

Furthermore, the subpaths and their cost to the destination nodes were also displayed. The algorithm's time complexity is O(V^2), where V represents the number of vertices in the graph. Additionally, the space complexity is also O(V^2) because a 2d matrix representation of the matrix was used, with data obtained from the input file downloaded from the Gset standard set of graphs that are used for testing and comparing different algorithms.

### Dataset:

Data used in this project is the standard set of graphs “G-set” that is often used for testing and comparison of various algorithms.The G-set could be accessed using the <a href="https://web.stanford.edu/~yyye/yyye/Gset/" style="display:inline-block;background-color:#8a8a8a;color:#fff;font-size:16px;padding:10px;border-radius:5px;text-decoration:none;">Stanford Libraries</a>.

About the Data:
1. The set picked in this project is the G1 set, which has 800 vertices and 19716 edges.
2. The weights associated with the edges were all 1.
3. To make the graph weighted, a list of randomly generated weights were edited into the third column, as shown in the image below.


![image](https://github.com/SaliElloh/dijkstra-s-algorithm/assets/112829375/c2681c19-4a0c-451c-ad28-c072dbdf6964)

 <small><b>Figure:</b> Vertex one and all the vertices connected to it are shown in the first and second column, respectively. The third column is the “weight” or the cost to get between vertex one (in this example) and the connecting vertices.</small>



### Algorithm explained:

Dijktra’s algorithm calculates the lowest cost or "cheapest way" to travel between two points or vertices in a <b>weighted graph</b>. The algorithm utilizes nodes to represent graph points and assigns them tentative distance values to determine the shortest path from the source node to other nodes in the graph.

The steps of the algorithm go as follows: 

1) Mark all vertices as unvisited, then create the unvisited set, which is a collection of all undiscovered nodes.
2) Assign a tentative distance value to each node: Mark all nodes with an infinity distance at first, except the source node, which is marked with a zero distance. Because no path is known between any other vertex aside from the source, all tentative distances have been originally set to infinity.
3) Consider all of your current node V's univisited neighbors U.
4) We update the cost[U] + weight of UV if it counts a lower cost than the existing cost[v].
5) We mark the code as visited and remove it from the unvisited collection once we have
finished taking into account all of the unvisited neighbors of this particular node. There will be no further visit to this node.
6) if the destination has been checked off as visited or if the shortest distance between nodes in the unvisited set is infinite, then the algorithm is then stopped. There is no connection between the node and the other nodes that haven't been visited.
7) As an alternative, we can choose the unvisited node marked with the least tentative distance, set it as the new current node, and then repeat these steps U–V times, or until all the vertices have been visited.

## Getting Started:

To get the project running, there's a few programs and steps needed.

### Built With:

Language used: [![C++](https://img.shields.io/badge/-C++-blue?style=flat&logo=C%2B%2B&logoColor=white)]()

IDE used: [![Built with Visual Studio Code](https://img.shields.io/badge/Built_with-Visual_Studio_Code-blue.svg)](https://code.visualstudio.com/)

### Prerequisites:

1. A C++ compiler such as GCC or Clang should be installed on your system.
2. A text editor or Integrated Development Environment (IDE) to edit and run the code. Ex: Visual Studio Code, Sublime Text, or Code::Blocks.
3. The standard C++ library should be available on your system, since the code uses C++ library headers,  which include <limits>, <vector>, <iostream>, and <fstream>.

### Steps to run the code:

 Download the "dijkstras-algorithm" zip file found in the uploaded files.
 
To do that, simply press on the zip file, then press "view raw" as shown below to download it:
![image](https://github.com/SaliElloh/dijkstra-s-algorithm/assets/112829375/01584c60-8d92-489e-b834-d8f05f16fe90)

    
## Results: 

This code was tested using three different source and destination vertices. The program outputted the distance cost of each subpath and the total cost for the path when source vertex 1 and destination node 150 were inputted. The same test was repeated for source vertex 1 and destination vertex 101, and source vertex 5 and destination vertex 80. 
    
![image](https://github.com/SaliElloh/dijkstra-s-algorithm/assets/112829375/ac6e43a1-61f9-4c6c-ad17-c6d9fc40d8ad)


<!-- LICENSE -->
## License:

No License used.

<!-- CONTACT -->
## Contact:

Sali E-loh - [@Sali El-loh](https://www.linkedin.com/in/salielloh12/) - ellohsali@gmail.com

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments:

* Special thanks to Professor Jin Lu at the University of Michigan - Dearborn for assigning and helping with this project in his Algorithm Analysis and Design class. 

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[LinkedIn.js]: https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white
[LinkedIn-url]: https://www.linkedin.com/in/salielloh12/






