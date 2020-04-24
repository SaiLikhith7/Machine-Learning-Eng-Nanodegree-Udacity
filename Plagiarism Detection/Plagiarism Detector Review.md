# Plagiarism Detector

Review date: 9 November 2019.



### Meets Specifications 

Dear student,
Congratulations on completing your Plagiarism Detector project! 🎉

You seem to have solid understanding of the topic and I wish you good luck with the capstone! 🙂



### All Required Files and Tests 

*The submission includes complete notebook files as `.ipynb`: "2_Plagiarism_Feature_Engineering" and "3_Training_a_Model". And the test and helper files are included: "problem_unittests.py", "helpers.py". The submission also includes a training directory `source_sklearn` OR `source_pytorch`.*

All required files included 👍

*All the unit tests in project have passed.*

Passed all unit tests in both notebooks 👍

<br>

### Notebook 2: DataFrame Pre-Processing 

*The function `numerical_dataframe` should be complete, reading in the original file_information.csv file and returning a DataFrame of information with a numerical `Category` column and new, `Class` column.*

Nice work 👍

<br>

*There is no code requirement here, just make sure you run all required cells to create a `complete_df` that holds pre-processed file text data and `Datatype` information.*

Great! 👍

<br>

### Notebook 2: Features Created 

*The function `calculate_containment` should be complete, taking in the necessary information and returning a single, normalized containment value for a given answer file.*

> ```
> for answer, source in zip(*array): temp_var.append(min(answer, source))
> ```

Nice one liner! 👍

<br>

*Provide an answer to the question about containment feature calculation.*

Right 👍

The normalized containment is calculated from the vocabulary of the source and answer texts alone.

*The function `lcs_norm_word` should be complete, taking in two texts and returning a single, normalized LCS value.*

I like how you used `enumerate` to extract the individual words right away! 👍

*Define an n-gram range to calculate multiple containment features. Run the code to calculate one LCS feature, and create a DataFrame that holds all of these feature calculations.*

> ```
> ngram_range = range(1,12)
> ```

Right, n-grams of 1 through 11 sound reasonable 🙂

<br>

### Notebook 2: Train and Test Files Created 

*Complete the function `train_test_data`. This should return only a *selection* of training and test features, and corresponding class labels.*

Clean coding work! 👍

*Select a few features to use in your final training and test data.*

> ```
> ['c_1', 'c_9', 'lcs_word']
> ```

👍

*Provide an answer that describes why you chose your final features.*

> Select feature with highest lcs_word and lowest correlation.

That's right. Also, by the nature of the task, having multiple measures of similarity is beneficial, thus including word-wise LCS feature as addition to any n-gram features is generally a good idea.

*Implement the `make_csv` function. The class labels for train/test data should be in the first column of the csv file; selected features in the rest of the columns. Run the rest of the cells to create `train.csv` and `test.csv`files.*

👍

<br>

### Notebook 3: Data Upload 

*Upload the `train.csv` file to a specified directory in an S3 bucket.*

👍

<br>

### Notebook 3: Training a Custom Model 

*Complete at least *one* of the `train.py` files by instantiating a model, and training it in the main if statement. If you are using a custom PyTorch model, you will have to complete the `model.py` file, as well (you do not have to do so if you choose to use an imported sklearn model).*

I think `RandomForestClassifier` is a great choice to start with.

It uses simple decision trees under the hood but mitigates their proneness to overfitting.

*Define a custom sklearn OR PyTorch estimator by passing in the required arguments.*

👍

*Fit your estimator (from the previous rubric item) to the training data you stored in S3.*

👍

<br>

### Notebook 3: Deploying and Evaluating a Model 

*Deploy the model and create a `predictor` by specifying a deployment instance.*

👍

*Pass test data to your deployed `predictor` and evaluate its performance by comparing its predictions to the true, class labels. Your model should get at least 90% test accuracy.*

> ```
> 0.96
> ```

Wohoo! 🎉

*Provide an answer to the two model-related questions.*

> We have 1 False Positive

Why do you think that is? I know it's hard to say, but generally there could be multiple overlapping reasons:

- the model is simply poorly optimized
- the 1-ngram containment feature could be too specific
- the mis-classified sample can be difficult to distinguish

<br>

### Notebook 3: Cleaning up Resources 

*Run the code to clean up your final model resources.*

👍

---

