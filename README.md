# Map_Navigator_in_C
 # Project: Map Navigator

## Description

The Map Navigator project consists of two programs: Map Maker and Map Navigator. These programs allow you to create a map of locations, specify directions between them, find paths, and calculate the shortest distance between nodes in the map.

### Map Maker

The Map Maker program lets you create a map by adding nodes (locations) and specifying the directions and distances between them. This program includes the following features:

- Add edges (connections) between nodes.
- Save the created map to a file for future use.
- Print the graph representation of the map.

### Map Navigator

The Map Navigator program allows you to perform various tasks on the created map, such as finding paths between nodes and calculating the shortest distance between them. This program includes the following features:

- Load a map from a file.
- Find paths between nodes.
- Print the map with directions and distances.
- Calculate the shortest distance between a source node and all other nodes in the map.

## Usage

### Map Maker

1. Run the Map Maker program.
2. Use the following options:
    - Add an edge: Specify the source and destination nodes, distance, and direction (right, left, straight, or back).
    - Save map to file: Save the created map to a file for future use.
    - Print graph: Display the current map representation.
    - Exit: Close the Map Maker program.

### Map Navigator

1. Run the Map Navigator program.
2. Enter the filename of the map to load.
3. Use the following options:
    - Find paths: Enter the source and destination nodes to find paths between them.
    - Print map: Display the map representation with directions and distances.
    - Find shortest distance: Calculate the shortest distance from a specified source node to all other nodes.
    - Exit: Close the Map Navigator program.

## Code Structure

### Map Maker (map_maker.c)

The Map Maker program contains the following key functions:

- `createNode`: Create a node with a specified data, distance, and direction.
- `createGraph`: Create a graph with a specified number of nodes (vertices).
- `addEdge`: Add an edge (connection) between two nodes.
- `printGraph`: Display the graph representation of the map.
- `saveMapToFile`: Save the map to a file.

### Map Navigator (map_navigator.c)

The Map Navigator program contains the following key functions:

- `createNode`: Create a node with a specified data, distance, and direction.
- `createGraph`: Create a graph with a specified number of nodes (vertices).
- `loadMapFromFile`: Load a map from a file.
- `findPaths`: Find paths between nodes using Depth-First Search (DFS).
- `printShortestPath`: Print the shortest path between nodes.
- `dijkstra`: Calculate the shortest distance using Dijkstra's algorithm.

## Compilation and Execution

To compile and execute the programs, use a C compiler. For example:

### Map Maker

```shell
gcc -o map_maker map_maker.c
./map_maker
```

### Map Navigator

```shell
gcc -o map_navigator map_navigator.c
./map_navigator
```

Make sure to follow the on-screen instructions and prompts to interact with the programs effectively.

## Note

- The programs use a simple text-based interface for interaction.
- The map is represented as a uni-directed graph.
- The distance is represented as an integer value.
- Directions are specified as "right," "left," "straight," or "back."


Feel free to contribute, modify, or distribute it as needed. Enjoy navigating your map!
