
 <center><h2>Machine Learning Course Coursera</h2></center>
This Module Covers : 
1. [[#What is machine learning]]
2. [[#Types of Machine Learning]]
3. [[#Supervised Learning]]
  - 3.1. [[#Regression]]
  - 3.2. [[#Classification]]
4. [[#Unsupervised Learning (without supervision)]]
  - 4.1. [[#Clustering Algorithm]] 
5. [[#Dimensionality Reduction]]
6. [[#Why Machine Learning]]
7. [[#Don't use Machine Learning When?]]

8. [[#Intermediary to Advance Terminologies]]
9. [[#Cross Validation]]
10. [[#Confusion Matrix]]
11. 
#### What is machine learning : 

Machine learning gives computer ability to learn without explicitly programmed **Arthur Samuel**

***Example :*** 
Checkers playing again and again and learning to play, and eventually became better than the famous checker player Arthur himself.

#### Types of Machine Learning

Two main types of Machine Learning are supervised and unsupervised learning: 

1. Supervised learning(used mostly in real world applications) course 1,2
2. Unsupervised learning
3. Reinforcement Learning


Having right kind and good amount of data, tools, and applying them efficiently and effectively is important for machine learning.

-> Machine learning Algorithms take much time.

-> Better to learn best practices throughout this course.

  
### Supervised Learning :
Supervised Learning refers to algorithms that learns x to y(input to output label), 

For this we have to give input X and their correct labels y.

-> Economic values are created by machine learning today

  

Examples : 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeG4xROCytwzzkM1HWKUhhZm5aSQ1_GbvZr8mJbZJ-XRJRdqectrGJ8vnd1_XdyvzZyzykSnefZ0siUZ8pnNcwjfUwKqTvQz67uD3Hffi2x8n2pB8QWUOGYQG72yoLEAS0Lf6-uNDCciTXc4KxZE1UIGjA?key=UrYzmsmRHfLYmCQJPTAPJA)

  

Given the input x(some emails) and their output y(spam or not spam)  to prediction models then we can test it on unseened input x(other emails) to check if it predict correct label(email is spam or not spam)

  

##### Regression : 
- **House Price Prediction by Regression :** 

Let's have a dataset having two columns Price of house in dollars, and house size in feets, both are drawn along x-axis(size of house) and y-axis(price in dollars), and data points are drawn on graph.

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcWuqLbS4ZsGIWg4BsSdBFgB3scOxa9Jw9u7IprSdBwucfzIiXbEgUqEOl6Mv6b2O6sGP8dsmJfNfZcHSXQrk2U-s34NQtHr7EjYJrZzvjTg97hNCJVEa3SQGfFvlnmL2m1IOoRP9idwhPyFCSJ7jkBdCE?key=UrYzmsmRHfLYmCQJPTAPJA)

  

Now if a person wants to buy a 750 square feet house and wants to predict it, the way of finding the best prediction is drawing a straight line such that it fits all the data points.(How? We will check later) Through this line we check corresponding y(price of house) value for desired x(size of house) value

**This machine learning is a type of supervised learning called regression.**

  

#### Classification : 
- **Breast Cancer Detection :** 

-> Building a tool that helps doctors diagnose breast cancer is an example of Classification.

-> Classification only has two possible outputs, or maybe more, but outputs are specific classes/categories.

This draws a boundary line between positive or negative tests.

So, later we can see by checking medical reports of patients to which boundary line they lie.  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVOQIL7K2KDd5010mgEt2FKoL-XLvVr9SYngmUnEbWP4c-JtUp6udeGqqJpje-T57yxCYQXhPQ5VP58qZlnAySsWBJTabcBjaoC_6XQZeP7zAXIDBif1mutfEW9Xm1jpwZlHEs0qNvIDXZcUR9gClaa_8?key=UrYzmsmRHfLYmCQJPTAPJA)


Blue circles show negative results

And Read cross shows positive results(have breast cancer)

I don’t know about medical tests. I use positive and negative only for understanding.  
  Where negative means tumor not found, which means no cancer, and if test is positive it means cancer.
  
Above one is 2D graph representation, and below is 1D graph representation by **dimensionality reduction.**

It is hard to classify at this point ‘?’(in image) whether the patient has positive or negative results.
For this we can check through 2D graph, by adding another feature ‘age’  

*Side Note : Keep an eye on image while reading*

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfL_D7_DnRkXJnOMofWZ3T7EMNv2BtdvDKQ3pYFYPepFV7ve8reldpGf8Gj_UL8bLlI0_CIlGF3A4hWY-d_sZzAcU5d90uFEFEmmEkuyp2QONt10i8A9gSFhboFHpi2QhKfxIBDlHLWiGNklYMu6Y8lqwAe?key=UrYzmsmRHfLYmCQJPTAPJA)

  

This helps make two separate classes that tell us that having more age and tumour size result in positive results for breast cancer, and obviously we can make more features to make it more accurate predictions.

### Unsupervised Learning (without supervision) : 
In unsupervised learning input(X) is given but labels to predict Y are not given in the dataset as examples like supervised learning.

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdHeA6HFUkgiYLLOsa9SS674Y3sjM8K4fvCgEhRrXVx8sV6ahCiX6-XKULYaaz_bXLJA2ETtHnXnxfkzfmA42qjc7lwlJX64tsGyDUl8DhMCAHPadnyfQBFhr9Afxj1ueebZoHJldHhZ-Oz-ScXO5fjWs9_?key=UrYzmsmRHfLYmCQJPTAPJA)

  
Our job is not to label them but is to find some structure, pattern or something interesting in unlabeled data.


-> In unsupervised Learning algorithms figure out by itself the patterns, or structures in the data.

### Clustering Algorithm : 

Make different Clusters based on density of data points.

Clustering is used in google news(recommending other related news, when we watch one).

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfOi-e3ZI945nvb-EHQnWE0WspuYh2rrziVKywqJncGJHjHdG_XCFjoVzbgK4NUn0bh86cmQCAnPTgiGhNhFE27wevv13yNIRDHX-vxCYKGFcWXFL3_ry6TU6BoG-hKfWOILDkqjLVg14PQvsd0NrN7d_I?key=UrYzmsmRHfLYmCQJPTAPJA)

  

In this case the algorithm has to figure out without supervision, to find news interesting for users, and bring related news to them.

  

- ***Clustering : DNA microarray***

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfb2gzvxiYpVqBrufJzzAg0KYxaWQ-CYbLS3i4qFJyXTfL8CCnKedABldxXcydGLgRqH9_-lBDZDFQdGYlsdJWDiRtlXBy2XxrTUYz5UKMVFwMNgLPjTKGYE3MEWE0ZaaGQa4Zfq-a6D1mtgITrPa5WyGE?key=UrYzmsmRHfLYmCQJPTAPJA)

Above image shows different characteristics of peoples,

Where columns represents separate people and rows represent their genetic characteristics, so algorithm can divide them into type1, type2, and type3, so this is called clustering.

*Note : Intensity of color may represent the difference of some of their characteristics.*

  
- ***Anomaly Detection :*** 
Used to detect unusual events or find unusual data points.
Applications of Anomaly Detection. Detect Unusual Bank Transactions

It is another benefit of clustering, to check if any thing is unusual than normal events, then it lies in an unusual event, and report it to bank owners.
  
### Dimensionality Reduction : 
Take a big dataset and compress it to a much smaller data set losing as little information as possible.



#### Difference Between Traditional Learning and Machine Learning

### Why Machine Learning

- **Intelligence***
-> Machine learning is used when intelligence is required in decision making, and logic is too complex to write using traditional programming approaches.

-> Think of Machine learning as a way to generate solutions or discover patterns using data. on the other hand Traditional programming relies on strict rules, which means always that predefined rules are applied.
Note : Machine learning algorithms evaluates on mathematical functions to make some decision according to the data.

- ***Complex Problems***
-> Now simple rules, can't process email text to check if the email is spam or not, Simple rules can't classify images, and can't recognize speech, as well as they can't process on large data to find patterns, and do some forecasting or predictions, as machine learning algorithms do.

-> It is important to note that It is not necessary to try to solve all problems using machine learning techniques, as they need a large amount of data, Use traditional approach when the problem is easily written in the form of code and there are less complexities in terms of problem solving.


- There are other reasons to be added here.

### Don't use Machine Learning When?
- Problem is well-defined and can be easily solved using simple rules.
- Insufficient data or low-quality data to train a model
- Not much resources are available for training on such data.



#### Intermediary to Advance Terminologies

### Cross Validation
Cross validation allows us to compare different machine learning methods and get a sense of how well they will work in practice.

The basic life cycle of machine learning algorithms is training the model on dataset, and then testing on dataset.

Generally we to take first 70-80% of data for training, and remaining 20-30% for testing.

Even if we take data for training in random order we don't know if the data is best(contains all possible records) for training.
In order to know it we use cross validation that divides the data into folds of equal sizes, and then experiment by considering some folds for training, and one fold for testing.
At last we can compare the result from all different combinations, and choose the most appropriate one.

It is common to divide data into 10 blocks, this is called Ten-Fold Cross Validation.



### Confusion Matrix

Confusion matrices are primarily used in classification tasks to evaluate the performance of the classification model.

Confusion matrix for a patient having a heart disease can be made as

![](Pasted%20image%2020241120175634.png)

![](Pasted%20image%2020241120175958.png)

![](Pasted%20image%2020241120180018.png)


![](Pasted%20image%2020241120180032.png)

![](Pasted%20image%2020241120180117.png)


Simply True, and False indicates the column predicted it right, or wrong
and Positive and negative indicates about positive and negative results of the heart disease.


So the number of correct predictions are in True Diagonal, which is always be one, and wrong predictions are in False Diagonal, which are always be all other diagonals than true.(In this case it is one because we only have two classes, if we have multiple classes, than number of diagonals must be higher)


Example : True(correct predictions) diagonal is one while all others are False Predictions.

|Predicted Class 1|Predicted Class 2|Predicted Class 3|
|---|---|---|

|   |   |   |   |
|---|---|---|---|
|**Actual Class 1**|TP (Class 1)|FP (Class 2)|FP (Class 3)|

|   |   |   |   |
|---|---|---|---|
|**Actual Class 2**|FP (Class 1)|TP (Class 2)|FP (Class 3)|

|                    |              |              |              |
| ------------------ | ------------ | ------------ | ------------ |
| **Actual Class 3** | FP (Class 1) | FP (Class 2) | TP (Class 3) |


### BIAS
