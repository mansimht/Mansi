What is a model?

A model is like a function that takes an input and gives the output.
Let f(x) be the function with x as input and the output is ‘y’. In regression, y is found to be continuous whereas in classification, y is found to be categorical or discrete.

What is discrete and continuous?

Discrete: In email spam detection the output will be “whether the email is spam or not “.
Continuous: Given the features, the predicted height of a person in the class is continuous. (As height can be anything between 140cm to 190 cm.)


1.Binary class classification: Classification with two class labels.
2.Multi-class classification: Classification with more than two class labels.

Algorithms:

1.Logistic Regression:
The name Logistic Regression sounds like a regression model but it does classification.
In this we try to find a Line(in 2D),Plane(in 3D),hyperplane(in nD) that separates the data points.
Let's assume there are two labels called +ve and -ve then all the +ve’s will be one side of the plane and all the -ve’s will be on other side of the plane.

2.K Nearest Neighbor’s(K-NN):
Compute the k nearest neighbor's distances and do a majority vote on the obtained ones.
The distance measure can be Euclidean, Manhattan, Minkowski, Hamming distance and cosine similarity distances. Taking a particular distance measure is problem specific.

3.Naive Bayes:

It is an elegant probabilistic approach. Let us assume we have three class labels namely C1, C2, C3.
We compute by using Bayes theorem that we learned in our 12th Standard:

P(C1|x) → Probability of class label C1 given a data point x.
P(C2|x) → Probability of class label C2 given a data point x.
P(C3|x) → Probability of class label C3 given a data point x.

Whichever is having the highest probability then the point belongs to that class.

4.Decision Trees:
It is a tree-like structure with a root node, internal nodes or decision nodes, leaf node(have class label). Splitting a node is based on Information gain(Ig). We calculate Information gain by using entropy or Gini Impurity. Splitting goes on until the entropy of the branch becomes zero(happens at a leaf node).
5.Random Forest Decision Tree’s:
Multiple decision trees are constructed by sampling(both row and column sampling with replacement) from the data and these decision trees are aggregated to produce the result. The result is based on the majority vote that are obtained from the multiple decision trees. This is an extremely parallelizable algorithm.

6.Support Vector Machines(SVM):
The key idea of the support vector machine is to find a plane that maximizes the margin such that the points are separated as widely as possible (or) we can construct the convex hulls for the points and find the shortest line connecting the hulls. Finally, bisect that shortest line.




