# Introduction

## What is Machine Learning?

- Arthur Samuel(1959). Machine Learning: Field do study that gives computers the ability to learn without being explicitly programmed

- Tom Mitchell(1998) Well-posed Learning Problem: A computer is said to learn from experience E with respect to some task T and some performance measure P, if its performance on T,as measured by P, improved with experience E.

## Supervised Learning

- In supervised learning, we are given a data set and already know what our correct output should look like, having the idea that there is a relationship between the input and the output

- Types of Supervised Learning Problems
  - **Classification**: trying to predict results in a discrete output. In other words, we are trying to map input variables into discrete categories.

    For example, given a patient with a tumor, we have to predict whether the tumor is malignant or benign.

  - **Regression**: trying to predict results within a continuous output, meaning that we are trying to map input variables to some continuous function
  
    For example, given a picture of a person, we have to predict their age on the basis of the given picture

## Unsupervised Learning

- Unsupervised learning allows us to approach problems with little or no idea what our results should look like. We can derive structure from data where we don't necessarily know the effect of the variables.

- We can derive this structure by clustering the data based on relationships among the variables in the data.

- With unsupervised learning there is no feedback based on the prediction results.

Example:

  - Clustering: Take a collection of 1,000,000 different genes, and find a way to automatically group these genes into groups that are somehow similar or related by different variables, such as lifespan, location, roles, and so on.

  - Non-clustering: The "Cocktail Party Algorithm", allows you to find structure in a chaotic environment. (i.e. identifying individual voices and music from a mesh of sounds at a cocktail party).