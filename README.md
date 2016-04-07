# BTM-Java
A java implement of Biterm Topic Model.  The origin BTM is in here: https://github.com/xiaohuiyan/BTM
Usage:
========
```java BTM [data_path] [topic_num] [alpha] [beta] [iter_num] [instance_num]```

* `[data_path]    string, path of training docs`
* `[topic_num]    int, number of topics`
* `[alpha]    double, Symmetric Dirichlet prior of P(z)`
* `[beta]   double, Symmetric Dirichlet prior of P(w|z)`
* `[iter_num]   int, number of iterations of Gibbs sampling`
* `[instance_num]   int, number of times to run this program`

Examples
========
```java BTM sample-data/sample-data.txt 100 0.1 0.01 2000 1```

Output
========
* `'model-final.theta'  Doc*Topic matrix`
* `'model-final.phi'  Topic*Word matrix`
* `'model-final.twords'  top 20 words of each topics`
* `'model-final.wordmap'  word dictionary`
