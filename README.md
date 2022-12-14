# A2-basic-stats-set2
## Topics: Normal Distribution, Functions of Random Variables
## 1.The time required for servicing transmissions is normally distributed with mu = 45 minutes and std = 8 minutes. The service manager plans to have work begin on the transmission of a customer’s car 10 minutes after the car is dropped off and the customer is told that the car will be ready within 1 hour from drop-off. What is the probability that the service manager cannot meet his commitment?
A) 0.3875 B) 0.2676 C) 0.5 D) 0.6987

Ans -[B] The servicing will begin after 10 mins of drop-off so 45+10 which will now take more than usual time so the new time (mew) is 55 min and the probability that it will take more than one hour to complete is "mew = 55, std = 8, q1 = stats.norm.cdf(60, loc=mew, scale = std), q1 = 0.266" The probability that the service manager cannot meet his requirement is 0.266.

## 2.The current age (in years) of 400 clerical employees at an insurance claims processing center is normally distributed with mean = 38 and Standard deviation =6. For each statement below, please specify True/False. If false, briefly explain why.
A)More employees at the processing center are older than 44 than between 38 and 44.
B)A training program for employees under the age of 30 at the center would be expected to attract about 36 employees.
Ans A - False, Because the probability for employees at the processing center are more between 38 and 44 than older than 44.

Ans B - True.

## 3.If X1 ~ N(μ, σ^2) and X2 ~ N(μ, σ^2) are iid normal random variables, then what is the difference between 2 X1 and X1 + X2? Discuss both their distributions and parameters.
Ans:The Normal Distribution has its link with the Central Limit Theorem, which states that ‘Any large sum of independent identically distribution random variables are approximately Normal then (X1 + X2) and (2X1) tends to have Normal distribution only If X1 and X2 are i.i.d and n is Large. The Difference between 2X1 and (X1 + X2) is the magnitude they hold of two different sample subsets (X1 and X2) from the same source(population). X1 and X2 can be a different subset of a sample from a similar source (population) but If X1 ~ N(μ, σ2) then, 2 X1 ~ N(2 μ, 4 σ2 ) If X1 ~ N(μ, σ2) and X2 ~ N(μ, σ2) are iid normal random variables then (X1 + X2)N(μ+ μ, σ2+ σ2)(2 μ, 2 σ2) Hence, 2X1 – (X1+X2) ~(2 μ – 2 μ, 4 σ2 + 2σ2 ) The distribution remains the same for every sample subset of similar source, it tends to fall under Normal distribution and slight deviations in parameters.

The Normal distribution has two parameters, the mean, µ, and the variance, σ2. µ and σ2satisfy −∞ < µ < ∞, σ2> 0. We write X ∼ Normal (µ, σ2) or X ∼ N(µ, σ2 ).

## 4.Let X ~ N(100, 20^2). Find two values, a and b, symmetric about the mean, such that the probability of the random variable taking a value between them is 0.99.
A)90.5, 105.9 B)80.2, 119.8 C)22, 78 D)48.5, 151.5 E)90.1, 109.9

Ans D - The two values of a and b, symmetric about the mean, are such that the probability of the random variable taking a value between them is 0.99 .""mew = 100, std = 20, np.round(stats.norm.interval(0.99, loc = 100, scale = 20),1))"" The two values of a and b, symmetric about the mean, are such that the probability of the random variable taking a value between them is 0.99: [ 48.5 151.5]"

## 5.Consider a company that has two different divisions. The annual profits from the two divisions are independent and have distributions Profit1 ~ N(5, 32) and Profit2 ~ N(7, 42) respectively. Both the profits are in Dollars Million. Answer the following questions about the total profit of the company in Rupees. Assume that $1 = Rs. 45
A) Specify a Rupee range (centered on the mean) such that it contains 95% probability for the annual profit of the company.
B) Specify the 5th percentile of profit (in Rupees) for the company
C) Which of the two divisions has a larger probability of making a loss in a given year?
Ans A -Rupee Ranges from 2.2 to 21.8 Million$ in Annual profit of the Company 95% of the time.

Rupee Ranges from 9.9 to 98.1 Crore Rupees in Annual profit of the Company 95% of time.

Ans B - The 5th percentile of Profit for the company is 3.78 Million$.

The 5th percentile of Profit for the company is 17.0 Crore Rupees.

Ans C - The Probability of Division 1 making a loss is 4.78 %

The Probability of Division 1 making a loss is 4.01 %

The Division 1 has a larger Probability of making a loss
