# Math 132A Project 1

##### By Teo Zeng, Angelica Zheng

## Cover Page

## Description of the Problem

A big car manufacturer produces different types of automobiles, including trucks, small cars, and midsized luxury cars. One of the company's plants, located near Detroit, MI, puts together two kinds of midsized luxury cars. The first model, known as the Family Adventurer, is a four-door sedan that comes with standard features, vinyl seats, plastic interior, and great gas mileage. It is promoted as a wise purchase for middle-class families who are on a tight budget, and every sale of the Family Adventurer earns the company a modest profit of 3,700 dollars. The second model, the Classic Transporter, is a two-door luxury sedan that has custom features, navigational capabilities, leather seats, and a wooden interior. It is advertised as a symbol of wealth for upper-middle-class families, and each sale of the Classic Transporter generates a profit of 5,300 dollars for the company.

At present, William Smith, who is in charge of the plant, is in the process of determining the manufacturing plan for the upcoming month. He must make a decision on the number of Family Adventurers and Classic Transporters to be produced in the plant to maximize the company's profits. He is aware that the plant has a labor-hour capacity of 48,500 hours for the month. Additionally, he knows that it takes 6 hours of labor to assemble one Family Adventurer, and 10.5 hours of labor to build one Classic Transporter.

The assembly plant, which William manages, does not manufacture the parts required to put together the two car models. Instead, these parts are delivered from other supplier plants located in Michigan. The car parts, such as tires, windows, doors, steering wheels, and seats, are transported to the assembly plant. For the upcoming month, William is aware that only 20,000 doors will be obtainable from the door supplier. The doors are used in both the Family Adventurer and the Classic Transporter, and the supplier plant was recently impacted by a labor strike, causing the factory to shut down for a few days. As a result, the supplier plant will not be able to fulfill its monthly production quota. The 20,000 doors include 10,000 left-hand doors and 10,000 right-hand doors.

The company has recently projected the monthly demand for various car models, and the forecast indicates that the demand for the Classic Transporter will be restricted to 3,500 cars. In contrast, there are no limits on the demand for the Family Adventurer, as long as the production capacity of the assembly plant is not exceeded.

## Model

We will use linear programming to model our problem, and we will first check that our problem satisfies the four assumptions of linear programming. According to the lecture notes, we have

1. **Proportionality**: which means that each decision variable in every equation must appear with a constant coefficient.
2. **Additivity**: the combined effect of the decision variables in any constraint or in the objective function is the algebraic sum of their individual weighted effects. (The weighting, of course, is due to the proportionality constants.)
3. **Divisibility or continuity**: the decision variables can take on fractional (non-integer) values.
4. **Certainty**: all model parameters (that is, the coefficients of the objective function, the coefficients of the constraints) are known deterministically (with certainty).

Having checked that our problem satisfies all four assumption of linear programming, let 

$x_1$ be the number of Family Adventurers to be produced.

$x_2$ be the number of Classic Transporters to be produced. 

$z$ be the profit to be maximized

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

## Interpretation of the Solution

## Recommendations