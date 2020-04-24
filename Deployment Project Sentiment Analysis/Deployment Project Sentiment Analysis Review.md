# Deploying a Sentiment Analysis Model

Review date: 29 September 2019.



### Meets Specifications 

Kudos ! I think you've done a good job of implementing the sentiment analysis model. Your concepts and usage of AWS Sagemaker and sentiment analysis are quite clear and have been well implemented in the notebook.

Further Resource: Keras has a neat API for visualizing the architecture, which is very helpful while debugging your network. [`pytorch-summary`](https://github.com/sksq96/pytorch-summary/) is a [similar project](https://github.com/sksq96/pytorch-summary/) in PyTorch.

Further, AWS Sagemaker recently got a [new update](https://aws.amazon.com/blogs/machine-learning/amazon-sagemaker-now-comes-with-new-capabilities-for-accelerating-machine-learning-experimentation/). It lets you find and evaluate the most relevant model training runs from the hundreds and thousands of your Amazon SageMaker model training jobs.

And Congratulations ![:tada:](https://review.udacity.com/assets/images/emojis/tada.png) once again, for successfully completing the project.



### Files Submitted 

*The submission includes all required files, including notebook, python scripts, and html files.*



### Preparing and Processing Data 

*Answer describes what the pre-processing method does to a review.*

Awesome. Correctly explained all the pre-processing steps by `review_to_words`.

*Answer describes how the processing methods are applied to the training and test data sets and what, if any, issues there may be.*

*The `build_dict` method is implemented and constructs a valid word dictionary.*

Awesome. Well done on this one. You took your time out to explain how the processing methods are applied to the training and test data sets.

*Notebook displays the five most frequently appearing words.*

Awesome. Correctly displays the five most frequently appearing words.



### Build and Train a PyTorch Model 

*The train method is implemented and can be used to train the PyTorch model.*

*The RNN is trained using SageMaker's supported PyTorch functionality.*



### Deploy a Model for Testing 

*The trained PyTorch model is successfully deployed.*



### Use the Model for Testing 

*Answer describes the differences between the RNN model and the XGBoost model and how they perform on the IMDB data.*

Awesome. Good job taking out this opportunity to write down your view of random tree models vs neural networks.

*The test review has been processed correctly and stored in the `test_data` variable.*

*The `predict_fn()` method in `serve/predict.py` has been implemented.*



### Deploying a Web App 

*The model is deployed and the Lambda / API Gateway integration is complete so that the web app works (make sure to include your modified `index.html`).*

*Answer gives a sample review and the resulting predicted sentiment.*

Awesome. The review looks reasonable, as does the resulting sentiment. Great!

---

