# greedy_machine_teaching_and_knn_classifiers

Author: Sui Jiet Tay

Code: main.ipynb

Premise: To compare the time complexity and "parameter loss measure" between a normal enumeration method vs a greedy algorithm for teaching point selection, and first glance at the KNN classifier.

- "Parameter loss measure"

$$
(\hat{a} - a)^{2} + (\hat{b} - b)^{2}
$$

> $a, b$ - parameters generated from the OLS Estimator from all $N$ data points of the training data

> $\hat{a}, \hat{b}$ - parameters generated from the OLS Estimator from $k$ data points of the teaching set, where $k\in N$. 

> $N$ - size of the training set

> $k$ - size of the teaching set, where k $\in$ $N$

- **Enumeration method**: For a teaching set of size $k$, enumerate all subsets of size $k$ from a set of training data, to yield the combination of data points with the best parameter loss. 
- **Greedy algorithm**: Pick a random data point as start point and incrementally selects the next optimal data point with the best smallest parameter loss measure from $N$ data points to be included in the teaching set of size $k$.

