# Map Of Denmark
This project was the focus of my second semester at ITU. The goad was to create an app that could read an OSM file and show an interactive map from the data. 

For this project, focus was placed on:
* Collaboration in small groups (5 people per group)
* Source control with Git and GitHub
* Effective use of relevant algorithms and data structures

My primary focus was on implementing and testing various spatial data structures. These included K-d trees, range trees, and R-trees. These data structures were used to determine which elements to render. The final product used a bulk-loading R-tree using Sort-Tile-Recursive (STR), as this implementation offered smaller minimum bounding rectangles (MBRs) and a lower number of nodes needed. 

![Comparison between R-Tree implementations](https://github.com/TheDavidNN/MapOfDenmark/images/RTreeComparison.png)
This image shows the resulting MBRs of a traditional R-tree, where elements were inserted one at a time (left), and a bulk-loaded R-Tree using STR (right).