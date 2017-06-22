# Predicting signed edges 

This notebook contains results from the work <span style="color:red">Predicting Positive and Negative Links: Theory & Applications</span></center>, authored by:
 
- **Charalampos E. Tsourakakis** (*Boston University, Harvard University*)
- **Michael Mitzenmacher** (*Harvard University*) 
- **Jaroslaw Blasiok** (*Harvard University*) 
- **Ben Lawson** (*Boston University*) 
- **Preetum Nakkira** (*Harvard University*) 
- **Vasileios Nakos** (*Harvard University*)

##  <center><span style="color:green">Feature construction </span></center>

The file *Constructing features.ipynb* demonstrates the construction of 
features used to predict the sign of an edge. The features we use include (a) the features proposed by [Leskovec et al](https://www.cs.cornell.edu/home/kleinber/www10-signed.pdf), (b) and the number of (positive, negative)x paths of length 3 and 4 respectively. Therefore, we add 4 new features. This notebook shows a quick implementation. We use the [Highland tribes](http://konect.uni-koblenz.de/networks/ucidata-gama) dataset from KONECT.  

##  <center><span style="color:green"> Sign Prediction </span></center>

In *Predicting Signed Edges.ipynb* we analyze the slashdot, and the wikipedia datasets from SNAP. We train a logistic regression classifer using stratified 10-fold cross-validation. We observe that paths are a very informative features, as our theoretical analysis justifies under certain probabilistic assumption. 
