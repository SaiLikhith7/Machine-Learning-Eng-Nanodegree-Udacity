# Capstone Proposal Review

Review date: 20 September 2019

<br>

### Meets Specifications 

You clearly have a solid understanding of your dataset and your approach to this problem. 

About the capstone project.

- This is essentially your last project to show off what you have learned throughout this program. Make sure you check out and follow the [capstone report template](https://github.com/udacity/machine-learning/blob/master/projects/capstone/capstone_report_template.md) and we look forward to seeing what you can create!

<br>

### Project Proposal 

*Student briefly details background information of the domain from which the project is proposed. Historical information relevant to the project should be included. It should be clear how or why a problem in the domain can or should be solved. Related academic research should be appropriately cited. A discussion of the student's personal motivation for investigating a particular problem in the domain is encouraged but not required.*

Very solid opening section here, as you have done a great job describing the problem and problem domain. Glad that you have chosen a real world problem and have referenced other research on such on a problem.

<br>

*Student clearly describes the problem that is to be solved. The problem is well defined and has at least one relevant potential solution. Additionally, the problem is quantifiable, measurable, and replicable.* 

> "The main objective of this capstone project is to take a first (small) step in the design of real time smart embedded system for environmental sound classification (ESC)."

Problem statement is clearly defined here. And glad that you mention that this would be a classification problem in this section.

<br>

*Student proposes at least one evaluation metric that can be used to quantify the performance of both the benchmark model and the solution model presented. The evaluation metric(s) proposed are appropriate given the context of the data, the problem statement, and the intended solution.*

Using accuracy is not the best for unbalanced datasets based on the [accuracy paradox](https://en.wikipedia.org/wiki/Accuracy_paradox), but since I looked at the distribution, accuracy is fine to use.

<br>

*The dataset(s) and/or input(s) to be used in the project are thoroughly described. Information such as how the dataset or input is (was) obtained, and the characteristics of the dataset or input, should be included. It should be clear how the dataset(s) or input(s) will be used in the project and whether their use is appropriate given the context of the problem.*

Ideally, you should also give some ideas in terms of the [distribution of the target class](https://machinelearningmastery.com/tactics-to-combat-imbalanced-classes-in-your-machine-learning-dataset/) in your training file. Do we have an unbalanced dataset? Balanced? Make sure you fully analyze the distribution of the target class, as this might determine what evaluation metric is appropriate in your problem and might be a big part of this particular dataset that you need to be aware of before diving in. 

But looking at other projects on this data, like
https://towardsdatascience.com/urban-sound-classification-part-1-99137c6335f9

I can see that the distribution isn't to unbalanced. 

[![Screen Shot 2019-09-19 at 7.03.47 PM.png](https://udacity-reviews-uploads.s3.us-west-2.amazonaws.com/_attachments/19273/1568945041/Screen_Shot_2019-09-19_at_7.03.47_PM.png)](https://udacity-reviews-uploads.s3.us-west-2.amazonaws.com/_attachments/19273/1568945041/Screen_Shot_2019-09-19_at_7.03.47_PM.png)



*Student clearly describes a solution to the problem. The solution is applicable to the project domain and appropriate for the dataset(s) or input(s) given. Additionally, the solution is quantifiable, measurable, and replicable.*

I think you have a good Solution Statement here, as it is clear that you have thought a lot about what your approach is to this problem. Mel-Frequency Cepstral Coefficients are a good idea.

<br>

*A benchmark model is provided that relates to the domain, problem statement, and intended solution. Ideally, the student's benchmark model provides context for existing methods or known information in the domain and problem given, which can then be objectively compared to the student's solution. The benchmark model is clearly defined and measurable.*

> "Salamon et [9] compares 5 different algorithms: decision tree (J48), k-NN (k = 5), random forest (500 trees), Support Vector Machine (SVM) (radial basis function kernel), and a baseline majority vote classier (ZeroR). The top performer is the SVM with a 67% classification accuracy for a 4 sec audio slice duration. The SVM will be used as benchmark model."

Using this external paper is a fine for a benchmark. Benchmarking is the process of comparing your result to existing method or running a very simple machine learning model, just to confirm that your problem is actually 'solvable'.

<br>

*Student summarizes a theoretical workflow for approaching a solution given the problem. A discussion is made as to what strategies may be employed, what analysis of the data might be required, or which algorithms will be considered. The workflow and discussion provided align with the qualities of the project. Small visualizations, pseudocode, or diagrams are encouraged but not required.*

You clearly have a good game plan in place here. Could also use some data augmentation. As this help the model actually 'learn' features and will also help increase the amount of data as well. If you would like to learn how to do this is straight tensorflow, check out this notebook

(https://github.com/Hvass-Labs/TensorFlow-Tutorials/blob/master/06_CIFAR-10.ipynb)

Could also even play around with [Test Time Augmentation (TTA)](https://towardsdatascience.com/test-time-augmentation-tta-and-how-to-perform-it-with-keras-4ac19b67fb4d).

<br>

*The proposal follows a well-organized structure and would be readily understood by its intended audience. Each section is written in a clear, concise and specific manner. Few grammatical and spelling mistakes are present. All resources used and referenced are properly cited.*

OK.

---

