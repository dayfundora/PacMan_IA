Pacman Search
===================

![Animated gif pacman game](http://ai.berkeley.edu/images/pacman_game.gif)

Artificial Intelligence search algorithm base on Pacman

### Source
[The Pacman Projects](http://ai.berkeley.edu/project_overview.html) by the [University of California, Berkeley](http://berkeley.edu/).

### Layouts
Different layouts can be found and created in the `layouts` directory

### Depth-First Search:
By running the following 4 commands, we can see the solutions for tinyMaze, mediumMaze, bigMaze and openMaze:
```
python pacman.py -l tinyMaze -p SearchAgent
python pacman.py -l mediumMaze -p SearchAgent
python pacman.py -l bigMaze -z .5 -p SearchAgent
python pacman.py -l openMaze -z .5 -p SearchAgent
```

### Breadth-First Search :
By running the following 4 commands, we can see the solutions for tinyMaze, mediumMaze, bigMaze and openMaze:
```
python pacman.py -l tinyMaze -p SearchAgent -a fn=bfs
python pacman.py -l mediumMaze -p SearchAgent -a fn=bfs
python pacman.py -l bigMaze -p SearchAgent -a fn=bfs
python pacman.py -l openMaze -p SearchAgent -a fn=bfs
```

### Iterative Deepening Search:
By running the following 4 commands, we can see the solutions for tinyMaze( any maze mediumMaze is fine):
```
python pacman.py -l mediumMaze -p SearchAgent -a fn=ids -z .5
```

### A* Search:
By running the following command, we can see the solutions for bigMaze with the manhattanHeuristic:
```
python pacman.py -l bigMaze -z .5 -p SearchAgent -a fn=astar,heuristic=manhattanHeuristic
```

### Corner's Problem:
By running the following  commands, we can see the solutions for the Corners Problem using Manhattan's minimum:
```
python pacman.py -l mediumCorners -p AStarCornersAgent -z 0.5
```

### Food Search Problem
For the solution in this code of Eating all the dots is used BFS to the Manhattan's maximum