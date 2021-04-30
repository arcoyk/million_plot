# million_plot
An example of million interactive points plot using three.js particle system for easy visualization of word2vec models.

![preview1](preview1.png)
![preview2](preview2.png)

Visualizing ./data/data.modul.js with [three.js](https://threejs.org/examples/?=interactive#webgl_interactive_points).

./data/data.module.js
```
var Data = [];
Data.ws = ["dog", "cat", ... "bird"];
Data.vs = [[10.32, 42.234], [54.234, 44.463], ... [23.532, 23.432]];
export {Data}
```

ws = words
vs = vectors

You can edit this file to change the visualizing data.

# Why?

This is convenient to grasp characteristic of word2vec models.