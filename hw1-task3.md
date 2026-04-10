# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> **Your Answer:**

- Regression, inference, n=200- observations, and p=5 predictors

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> **Your Answer:**

- Classification, prediction, n=30 obs. , and p= 12 predictors

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> **Your Answer:**

- Regression, prediction, n= 52 weekly data obs. , p= 5

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> **Your Answer:**

-Advantages: Potential to accurately fit a wider range of possible shapes for f.

-Disadvantages:Complex models could often lead to overfitting data. If the chosen model is too far off from true f, then the estimate will be poor.

When inference is the goal, linear models are a good choice since it is easy to understand the relationship between the variables (X,Y).
Flexible approaches are more difficult to interpret and can lead to a complicated estimate of f, by how any individual predictor is associated with response. 
A less flexible or more restrictive can produce just a relatively small range of shapes to estimate f. This can be used with GAMs, non-linear relationships. Less interpretable than linear regression.


### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> **Your Answer:**
Parametric - Two-Step Model-based approach, assumption about the functional form, or shape of f. A linear model, it reduces the problem of estimating f down to one of estimating a set of parameters

Disadvantage:  of a parametric approach is that the model we choose will usually not match the true unknown form of f. Cause overfitting, this follows the errors, or noise, too closely.

Advantage: Reduces the problem of estimating, f, down to one of estimating a set of parameteres. Generally easier to estimate a set of parameters in the linear model. Flexible models can fit many different functional forms for f

Non-Parametric: Does not make explicit assumptions about the functional form of f, it seeks an estimate of f that gets as close as to the data points as possible without being too rough or wiggly.

Advantages: Avoiding assumptoin of a particular function form of f, they have potential to accurately fit a wider range of posisble shapes for f. helps avoid fitting the data well.

Disadvantages: Do not reduce the problem of estimating f to a small # of parameters, a very large # of observations is required in order to obtain an accurate estimate of f.