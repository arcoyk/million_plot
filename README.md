# Million Plot
[DEMO](https://million-plot.glitch.me/)

![preview1](preview1.png)
![preview2](preview2.png)

A simple visualization of feature vectors and its metadata (Up to roughly 3 million points with MacBookPro 2019). In this example, feature vectors of a word2vec model was used with its words as metadata ([UMAP](https://arxiv.org/abs/1802.03426)-compressed [Japanese word2vec model](http://www.cl.ecei.tohoku.ac.jp/~m-suzuki/jawiki_vector/)) Replace ./data/data.module.js to visualize your data.

./data/data.module.js
```
var Data = [];
Data.ws = ["dog", "cat", ... "bird"];
Data.vs = [[10.32, 42.234], [54.234, 44.463], ... [23.532, 23.432]];
export {Data}
```

ws = words
vs = vectors

words and vectors must be corresponding. e.g. the point of "dog" appears at (x, y) = (10.32, 42.234) on the example above. The label appears with mouse hover.

# Why?
You can easily create interactive visualization systems for feature vectors using this repo. For simple visualization purpose, consider using [Embedding Projector](https://projector.tensorflow.org/). For more advanced visualization, see [Arts & Culture Experiment](https://artsexperiments.withgoogle.com/freefall). For more fewer points / coding consider using [p5.js](https://p5js.org/examples/form-points-and-lines.html). If you're looking for some graphs [D3.js](https://observablehq.com/@d3/scatterplot-matrix).