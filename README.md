# MathematicalFinanceModels
Learning and strengthening understanding of introductory math finance through implementation as a program
Basic structure will be a class representing a stock price, with several others
One will be a Brownian Motion with fields/data members:

  -Mean (always zero)
  -Variance (argument of constructor)
  -Method to return a random value from a Normal distribution with mean 0 and variance Variance
  
And a function for multiplying any two brownian motions or difference of brownian motions

Class for the stock price will be structured:

  Data Members: mu, sigma, t, T, N, S (S is price at time t)
  Constructor: mu, sigma, T, N, S, t = 0
  Constructor: mu, sigma, t, T, N, S
  
  Methods:
    - (no args) DiscretePrice, Return S_T, S_T = S*exp(mu*(T-t) + Sum(sigma*sqrt(Delta_T)*zeta)), 
    - ContinuousPrice, same as above, only S_T = S*exp(mu*(T-t) + sigma*B(T-t)), Bt is a brownian motion, or rather a random          value returned from a method on a BM object
  
