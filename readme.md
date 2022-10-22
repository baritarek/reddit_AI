## steps
1. to run q1 to  q2.4 add the goemotions zip to your root,simply step through the proj.ipynb notebook but avoid the blocks with grid-searches if you don't want to find the best parameters as we trained the models with
them already and then hard coded to prevent dependence on running gridsearch.Meaning you have the chance of running gridsearch again and using the values you find to replace the ones i hardcoded by playing the grid search blocks or trust the ones I found as legitimate.
2. we wrote a utility function that for q1 to 2.4 appends to a file called performance which I included the classification report and confusion matrix and after playing through the notebook
you should have all the models and result appended to the file (you might want to clear the file before rerunning if you wish to overwrite my reports)
3.  q2.5 is where we just added stop words removal, but to make it more readable and separate from earlier questions we extracted them out in a notebook of its own that can be run 
similarly to 1 to 2.4 . The only difference is that it writes its performance to a file called "performance 2.5"
4. To run part 3, you can just step the notebook labeled "q3" and will generate the models as desired (they save the output of their classification into the performance file). We have made functions that avergae the embeddings automatically so all you need to do is play through the notebook as stated relevant headings exist for each embedding and you can find their classification reports and confusion matrices in the performance file
