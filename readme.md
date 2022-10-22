# Repo 
1. link: https://github.com/baritarek/reddit_AI

## steps
Note: step assumes you have python installed and jupyter and have added goemotions.json.zip to the root of the project directory (you may need to use pip to install scikit learn,pandas,numpy,matplotlib,nltk,gensim and pickle) 
1. to run q1 to q2.4,simply step through the proj.ipynb notebook but avoid the blocks with grid-searches if you don't want to find the best parameters as we trained the models with
them already and then hard coded to prevent dependence on running gridsearch.Meaning you have the chance of running gridsearch again and using the values you find to replace the ones i hardcoded by playing the grid search blocks or trust the ones I found as legitimate.
2. we wrote a utility function called "write_matrix_and_report_to_file" that for q1 to 2.4 appends to a file called performance after predicting with x_test (this flow happens under the heading "classification reports and confusion matrices"), In this section of the notebook all played through models explained
above are fed the X_test values and write their results using the function  "write_matrix_and_report_to_file" to the performance file 
3.  q2.5.ipynb is where we just added stop words removal (q2.5 experimentation), but to make it more readable and separate from earlier questions we extracted them out in a notebook of its own that can be run 
similarly to 1 to 2.4 . The only difference is that it writes its performance to a file called "performance 2.5"
4. To run part 3, you can just play through the notebook labeled "q3.ipynb" and will generate the models and produce y_preds that will be passed to the "write_matrix_and_report_to_file" function similar to the other notebooks which saves metrics to the performance file. We have made functions that average the embeddings automatically so all you need to do is play through the notebook as stated. Relevant headings exist for each embedding but the first half of the notebook up
until "fasttext-wiki-news-subwords-300" prepares and trains the data and returns metrics for google-news embeddings.
