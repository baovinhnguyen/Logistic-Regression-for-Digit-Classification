# Logistic-Regression-for-Digit-Classification

The project objective is to use logistic regression to classify hand-written digits (8 and 9 in particular). First, I fitted logistic regression models to the training data using sklearn's implementation of the model with the liblinear solver. I explored what happens when limiting the iterations allowed for the solver when converging to its solution, leaving all other parameters with default values. 

I also explored different values of the inverse penalty strength C using a regularly-spaced grid of values logspace(-9, 6, 31). Then I determined what C value gives the least log loss on the test data. I also included accuracy score of the model and a confusion matrix. 

I analyzed the false positives and the false negatives and provided some thoughts about what mistake the classifier is making. 
 
Finally, I analyzed all of the final weights produced by the classifier. I reshaped the weight coefficients into a (28 × 28) matrix, corresponding to the pixels of the original images, and plot the result using imshow(), with colormap RdYlBu, vmin=-0.5, and vmax=0.5. I will discuss the plot regarding which pixels correspond to an 8 (have negative weights), and which correspond to a 9 (have positive weights).





