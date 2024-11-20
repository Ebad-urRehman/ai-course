### Linear Regression : 
- Most widely used algorithm contains many basics of machine learning.
- Regression model predicts numbers as the output.
- Linear regression is one example of a Regression model.

Example :  Predicting house prices as we do before.

Another type of supervised learning is *Classification*, in which categories are involved as outputs.

#### Some Terminologies : 

- Data used to train model -> training set(represented by X called input variable feature)
- Data used to test model -> test set(represented by y called output/target variable)
- m = number of training examples
- Single training examples can be represented as (x,y)
- (x<sup>i</sup>, y<sup>i</sup>) = ith training example (i in superscript)
- Training set going through a learning algorithm generates the function f.
- Training set generates a  Learning Algorithm that minimizes to generate a  function(f)

This functions looks like this
f(x) = wx + b
Or
f(x) = wb<sub>1</sub> +b<sub>0</sub>

Both are Same under different notations.
Where b<sub>0</sub> or w is slope of the line, and b<sub>1</sub> or b is y intercept.

This line upon giving the input x predicts the value of y. This means we put value of x in f(x) = wx + b and get the value of y.

This value of predicted y is represented as y<sup>^</sup> which means this value is approximated.

And it may be equal or less or very different from actual target value.

y<sup>^</sup> approximately equals to y

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcv8rPGwKrFfwm1V6fZmikfvT4hHR5474ZlTR6YXma68lo9vriiUNM5JP7K2VsY7eVY483Tx62OtpoBzEzr_iEBy2I9JCGvUsWFsGI_a_Zb-bfz-Sr7VPrMW_viBVnfjwoueaUH6M3Q7XZUahoO7exzNpIV?key=UrYzmsmRHfLYmCQJPTAPJA)

  
Univariate Regression : Regression in which we have only one input and output variable.

#### Implement Linear Regression : 

#### Cost Function : tells us how good our model is doing.

-> We have to find values of w and b, to find such a line in which in which y<sup>^</sup> is closer to y for all (x<sup>i</sup>, y<sup>i</sup>)

In order to find such values for w and b for such a line we need a *cost function*.

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdBZJ3NK4UYpUCSwQXhdtHDaxT05jmPxfoCeY-_PBEFZTX1QeWksAKi5TVPsK_qiAHA7KiUyeqERzX4AxGteRQ0vIbzjwn4NrasQ_Qh7C0lqUHD_F9NJnTfZOt6LZ6VqvCK6j_vPsbqbGHm89qsuQryQ6gW?key=UrYzmsmRHfLYmCQJPTAPJA)

Here the formula on the right+ shows the cost function.

#### Mean Square Error or Cost Function : 
We can say for every point we find the error which can be find by subtracting actual value from predicted value, and we square them because there may be negative values, and then add up all the values to get the sum of error for all training examples, then we can divide it by total number of training examples m, to get average of error called cost function.

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfL8PSwNNeO_kz14Cg3pvERxaf59wN-ZppNEUYNhrQYYVVsPLVyXebq_4NxKyfrT6MeJjHRh1iVgrsOaqCTwQxy4cNTpeJES2PuOT0ZOGATf2ra1tJW_EpBopZHPilsuHl1HLlci-Jn75x9XrfQ1cUxPsI?key=UrYzmsmRHfLYmCQJPTAPJA)

  
2 is also divided to make calculations look neater, and there is no effect on later calculations why? 🤔

This is also called the squared error cost function.(most commonly used cost function)


[[Gradient Descent]] is used in order to minimize the cost function easily.
If we are manually trying to find the best fit by changing values of w1 and b etc it would take much longer time, and it is more likely that we can never found the best fit.
