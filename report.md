# Math 132A Project 1

##### By Teo Zeng, Angelica Zheng

## Cover Page



## Description of the Problem

Our company produces different types of automobiles, including trucks, small cars, and midsized luxury cars. One of the company's plants, located near Detroit, MI, puts together two kinds of midsized luxury cars. The first model, known as the Family Adventurer, is a four-door sedan that comes with standard features, vinyl seats, plastic interior, and great gas mileage. It is promoted as a wise purchase for middle-class families who are on a tight budget, and every sale of the Family Adventurer earns the company a modest profit of 3,700 dollars. The second model, the Classic Transporter, is a two-door luxury sedan that has custom features, navigational capabilities, leather seats, and a wooden interior. It is advertised as a symbol of wealth for upper-middle-class families, and each sale of the Classic Transporter generates a profit of 5,300 dollars for the company.

At present we are in the process of determining the manufacturing plan for the upcoming month. We must make a decision on the number of Family Adventurers and Classic Transporters to be produced in the plant to maximize the company's profits. We are aware that the plant has a labor-hour capacity of 48,500 hours for the month. Additionally, we know that it takes 6 hours of labor to assemble one Family Adventurer, and 10.5 hours of labor to build one Classic Transporter.

The assembly plant does not manufacture the parts required to put together the two car models. Instead, these parts are delivered from other supplier plants located in Michigan. The car parts, such as tires, windows, doors, steering wheels, and seats, are transported to the assembly plant. For the upcoming month, William is aware that only 20,000 doors will be obtainable from the door supplier. The doors are used in both the Family Adventurer and the Classic Transporter, and the supplier plant was recently impacted by a labor strike, causing the factory to shut down for a few days. As a result, the supplier plant will not be able to fulfill its monthly production quota. The 20,000 doors include 10,000 left-hand doors and 10,000 right-hand doors.

Our company has recently projected the monthly demand for various car models, and the forecast indicates that the demand for the Classic Transporter will be restricted to 3,500 cars. In contrast, there are no limits on the demand for the Family Adventurer, as long as the production capacity of the assembly plant is not exceeded.

## Model

We will use linear programming to model our problem, and we will first check that our problem satisfies the four assumptions of linear programming. Let,

$x_1$ be the number of Family Adventurers to be produced.

$x_2$ be the number of Classic Transporters to be produced. 

$z$ be the profit to be maximized

Now our decision variable is $x_1$ and $x_2$ with objective function $ z = 3700x_1 + 5300x_2$

According to the lecture notes, we have

1. **Proportionality**: which means that each decision variable in every equation must appear with a constant coefficient.

> In our case, proportionality is satisfied because the contribution of our decision variables to the objective function is proportional to their values. For example, one Family Adventurer generates a profit of $3700$ dollars and two Family Adventurers generate profit of $7400$ dollars.

2. **Additivity**: the combined effect of the decision variables in any constraint or in the objective function is the algebraic sum of their individual weighted effects.

> In our case, additivity is satisfied because the contribution to the objective function for any of our variable is independent of the other decision variables. For example, the profit of each Family Adventurer will always be $3700$ dollars regardless the profit of each Classic Transporter. And vice versa.

3. **Divisibility or continuity**: the decision variables can take on fractional (non-integer) values.

> In our case, divisibility is satisfied because when the number of cars produced are fractional, we can round up or down to obtain an integer value to satisfy the integer requirement.

4. **Certainty**: all model parameters (that is, the coefficients of the objective function, the coefficients of the constraints) are known deterministically (with certainty).

> In our case, certainty is satisfied because we were given all constraints, coefficients, objective function of the linear programming problem, which are all deterministic.

Having checked that our problem satisfies all four assumption of linear programming

We formulate our problem as the following
$$
\begin{cases}
 		\text{Maximize  } \rightarrow z = 3700x_1 + 5300x_2\\
 		\text{Subject to:}\\
 		6x_1 +10.5x_2 \leq 48500\\
 		4x_1 + 2x_2 \leq 20000\\
 		x_2 \leq 3500\\
 		x_1 \geq 0, x_2 \geq 0
 \end{cases}
$$
As we can see in the formulation, we want to maximize the profit $z$, which is subject to individual profits of each car model. The first constraint was due to labor hours. The second constraint was due to car doors and the third constraint was brought by the company forecast.

## Solution of the Model

Now we will solve the problem using Excel:

![](/Users/teo/Desktop/math132a-project/imgs/excel.png)

We found that the optimal solution is when 
$$
\begin{cases}
 		x_1 = 3766\\ 
 		x_2 = 2467
 \end{cases}
$$
generating a profit of 
$$
3700 \times 3766 + 5300 \times 2467 = 27009300 \text{   dollars}
$$
To verify that the solution is unique, we plot out the feasible regions as shown below:

![](imgs/plot1.png)

We can see from the above plot, that the conditions form a polygon boundary. Since the objective function is not parellel to any of the boundary, there exists an unique optimal to this linear programming problem. Hence there exists an unique solution.

## Interpretation of the Solution



## Recommendations