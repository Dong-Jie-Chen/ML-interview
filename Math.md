# Mathematics - List of questions

## Linear Algebra
1. What is broadcasting in connection to Linear Algebra?
1. What are scalars, vectors, matrices, and tensors?
1. What is Hadamard product of two matrices?
1. What is an inverse matrix?
1. If inverse of a matrix exists, how to calculate it?
1. What is the determinant of a square matrix? How is it calculated (Laplace expansion)? What is the connection of determinant to eigenvalues?
    
    det(A) = λ1 · λ2 ····· λn the determinant is the product of the eigenvalues.
3. Discuss span and linear dependence.

  linear dependent: solve Ax=0
5. What is Ax = b? When does Ax =b has a unique solution? 

  rank(A)=n
7. In Ax = b, what happens when A is fat or tall?

  fat: 0 solution or infinite solution. tall: any solution
  
9. When does inverse of A exist?


  If the Det(A) is non zero then A^-1 exists. 
11. What is a norm? What is L1, L2 and L infinity norm?
13. What are the conditions a norm has to satisfy?

  non-negative
16. Why is squared of L2 norm preferred in ML than just L2 norm?

The squared Euclidean norm is widely used in machine learning partly because it can be calculated with the vector operation xTx.
18. When L1 norm is preferred over L2 norm?

the L2 norm squares values, so it increases the cost of outliers exponentially; the L1 norm only takes the absolute value, so it considers them linearly.

20. Can the number of nonzero elements in a vector be defined as L0 norm? If no, why?
21. What is Frobenius norm?

cycle through all matrix entries, add their squares, and then take the square root
23. What is a diagonal matrix? (D_i,j = 0 for i != 0)
24. Why is multiplication by diagonal matrix computationally cheap? How is the multiplication different for square vs. non-square diagonal matrix?
 
!!!!!
27. At what conditions does the inverse of a diagonal matrix exist? (square and all diagonal elements non-zero)
28. What is a symmetrix matrix? (same as its transpose)
29. What is a unit vector?
30. 
31. When are two vectors x and y orthogonal? (x.T * y = 0)
32. At R^n what is the maximum possible number of orthogonal vectors with non-zero norm?
33. When are two vectors x and y orthonormal? (x.T * y = 0 and both have unit norm)
34. What is an orthogonal matrix? Why is computationally preferred? (a square matrix whose rows are mutually orthonormal and columns are mutually orthonormal.)
35. What is eigendecomposition, eigenvectors and eigenvalues?
36. How to find eigen values of a matrix?
37. Write the eigendecomposition formula for a matrix. If the matrix is real symmetric, how will this change?
38. Is the eigendecomposition guaranteed to be unique? If not, then how do we represent it?
39. What are positive definite, negative definite, positive semi definite and negative semi definite matrices?
40. What is SVD? Why do we use it? Why not just use ED?
41. Given a matrix A, how will you calculate its SVD?
42. What are singular values, left singulars and right singulars?
43. What is the connection of SVD of A with functions of A?
44. Why are singular values always non-negative?
45. What is the Moore Penrose pseudo inverse and how to calculate it?
46. If we do Moore Penrose pseudo inverse on Ax = b, what solution is provided is A is fat? Moreover, what solution is provided if A is tall?
47. Which matrices can be decomposed by ED? (Any NxN square matrix with N linearly independent eigenvectors)
48. Which matrices can be decomposed by SVD? (Any matrix; V is either conjugate transpose or normal transpose depending on whether A is complex or real)
49. What is the trace of a matrix?
50. How to write Frobenius norm of a matrix A in terms of trace?
51. Why is trace of a multiplication of matrices invariant to cyclic permutations?
52. What is the trace of a scalar?
53. Write the frobenius norm of a matrix in terms of trace?

## Numerical Optimization
1. What is underflow and overflow? 
1. How to tackle the problem of underflow or overflow for softmax function or log softmax function? 
1. What is poor conditioning? 
1. What is the condition number? 
1. What are grad, div and curl?
1. What are critical or stationary points in multi-dimensions?
1. Why should you do gradient descent when you want to minimize a function?
1. What is line search?
1. What is hill climbing?
1. What is a Jacobian matrix?
1. What is curvature?
1. What is a Hessian matrix?

## Basics of Probability and Informaion Theory
1. Compare "Frequentist probability" vs. "Bayesian probability"?
1. What is a random variable?
1. What is a probability distribution?
1. What is a probability mass function?
1. What is a probability density function?
1. What is a joint probability distribution?
1. What are the conditions for a function to be a probability mass function?
1. What are the conditions for a function to be a probability density function?
1. What is a marginal probability? Given the joint probability function, how will you calculate it?
1. What is conditional probability? Given the joint probability function, how will you calculate it?
1. State the Chain rule of conditional probabilities.
1. What are the conditions for independence and conditional independence of two random variables?
1. What are expectation, variance and covariance?
1. Compare covariance and independence.
1. What is the covariance for a vector of random variables?
1. What is a Bernoulli distribution? Calculate the expectation and variance of a random variable that follows Bernoulli distribution?
1. What is a multinoulli distribution?
1. What is a normal distribution?
1. Why is the normal distribution a default choice for a prior over a set of real numbers?
1. What is the central limit theorem?
1. What are exponential and Laplace distribution?
1. What are Dirac distribution and Empirical distribution?
1. What is mixture of distributions?
1. Name two common examples of mixture of distributions? (Empirical and Gaussian Mixture)
1. Is Gaussian mixture model a universal approximator of densities?
1. Write the formulae for logistic and softplus function.
1. Write the formulae for Bayes rule.
1. What do you mean by measure zero and almost everywhere?
1. If two random variables are related in a deterministic way, how are the PDFs related?
1. Define self-information. What are its units?
1. What are Shannon entropy and differential entropy?
1. What is Kullback-Leibler (KL) divergence?
1. Can KL divergence be used as a distance measure?
1. Define cross-entropy.
1. What are structured probabilistic models or graphical models?
1. In the context of structured probabilistic models, what are directed and undirected models? How are they represented?
What are cliques in undirected structured probabilistic models?

## Confidence interval
1. What is population mean and sample mean?
1. What is population standard deviation and sample standard deviation?
1. Why population s.d. has N degrees of freedom while sample s.d. has N-1 degrees of freedom? In other words, why 1/N inside root for pop. s.d. and 1/(N-1) inside root for sample s.d.? (Here)
1. What is the formula for calculating the s.d. of the sample mean?
1. What is confidence interval?
1. What is standard error?
