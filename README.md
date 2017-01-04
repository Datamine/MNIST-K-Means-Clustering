# MNIST-K-Means-Clustering
Using K-Means Clustering to Identify Handwritten Digits

Uncompress the .tar.gz archive to get the `digits.base64.json` dataset, which you'll need. (`tar -xzvf digits.base64.json.tar.gz`)

Design decision: the clustering algorithm is designed to train on labelled data. However, I've written it in such a way that it's easy to
change to unlabelled data -- I considered making it modular for labelled/unlabelled data, but the more I think about it, the less I'm convinced
of the utility of having a k-means clustering algorithm for unlabelled training data. (If your data is unlabelled, you can just place a dummy label on every datapoint.)

Inspired by a homework assignment in John Lafferty's [Large-Scale Data Analysis](https://galton.uchicago.edu/~lafferty/37601-syllabus.pdf) course that I took at UChicago in the Spring of 2015. I collaborated with Elliott Ding on that assignment. In the class, we used distributed systems via AWS and Apache Spark, parallellized code, and did most analysis using map-reduce. To make the computational statistics more accessible, I've rewritten this notebook to not use distributed techniques.

-----

See my blog post on this project [here](http://johnloeber.com/docs/kmeans.html).
