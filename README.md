# million_plot
An example of million interactive points plot using three.js particle system for easy visualization of word2vec models.

![preview1](preview1.png)
![preview2](preview2.png)

Visualizing ./data/data.modul.js using [three.js interactive particle example](https://threejs.org/examples/?=interactive#webgl_interactive_points).

./data/data.module.js
```
var Data = [];
Data.ws = ["dog", "cat", ... "bird"];
Data.vs = [[10.32, 42.234], [54.234, 44.463], ... [23.532, 23.432]];
export {Data}
```

ws = words
vs = vectors

words and vectors must be corresponding. e.g. the point of "dog" appears at (x, y) = (10.32, 42.234) on the example above. Label appears with mouse hover.

You can edit this file to change the visualizing data. In this example, data.module.js is [UMAP](https://arxiv.org/abs/1802.03426)-compressed [Japanese word2vec model](http://www.cl.ecei.tohoku.ac.jp/~m-suzuki/jawiki_vector/). 

# Why?

This is convenient to grasp characteristic of word2vec models.