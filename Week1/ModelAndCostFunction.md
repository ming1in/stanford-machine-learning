# Model and Cost Fucntion

## Model Representation

- Notation
  - *x<sup>(i)</sup>* : 'input' variable or **input features**
  - *y<sup>(i)</sup>* : 'output' or **target variable** that we are trying to predict
  - *(x<sup>(i)</sup> , y<sup>(i)</sup>)* : as a pair it is called a **training example** from the dataset
  - *(x<sup>(i)</sup> , y<sup>(i)</sup>); i = 1, ...,m* : a **training set** comprised of a list of training examples
  - *X* : denote all the input values
  - *Y* : denote all the output values
  - *h* : denotes a hypothesis or relation between *X* and *Y*
  - $\theta$ : a parameter of the hypothesis function

- The superscript *i* in the above notation is simply an idex into the training set and has nothing to do with exponentiation

- A more formal definition of supervised learning problems is given training, learn a function *h : X -> Y* so that *h(x)* is a 'good' predictor for the corresponding *y* value.

- If the target variable that we are trying to predict is continuous, then the learning problem is a **regression problem**.

- When *y* can take on only a small number of discrete values, then it is a **classification problem**

## Hypothesis Function

- Given a hypothesis function *h<sub>$\theta$</sub>(x) = $\theta$<sub>0</sub> + $\theta$<sub>1</sub>x* with parameters *$\theta$<sub>0</sub>* and *$\theta$<sub>1</sub>*
  - If *$\theta$<sub>0</sub> = 1.5* and *$\theta$<sub>1</sub> = 0*, then the hypothesis function will be a constant value function

  - If *$\theta$<sub>0</sub> = 0* and *$\theta$<sub>1</sub> = 0.5*, then the hypothesis function will be linear function with slope 0.5

  - If *$\theta$<sub>0</sub> = 1* and *$\theta$<sub>1</sub> = 0.5*, then the hypothesis function will be linear function with slope 1 and y-intercept 0.5

## Cost Function

- The cost function is used to measure the accuracy of a hypothesis function

- It take the average difference of all the results of the hypothesis with inputs from *X* and the actual output *y*

- The Square error function or Mean square error is...
  
  *J( $\theta$<sub>0</sub>, $\theta$<sub>1</sub> ) = $\frac{1}{2m}$ $\sum_{i=0}^{m}$ ( h<sub>$\theta$</sub> ( x<sub>i</sub> ) - y<sub>i</sub> )*

  In simpler terms, it is *$\frac{1}{2} \bar{x}$* where *$\bar{x}$* is the mean of the squares between *h<sub>$\theta$</sub> ( x<sub>i</sub> ) - y<sub>i</sub>*, or the difference between the predicted value and the actual value.

  The mean is halved as a convenience for the computation, the derivative of the square term will cancel ouy the $\frac{1}{2}$.

  ![Mean Square Error](images/MeanSquareError.png)
  
## Cost Function Intuition
