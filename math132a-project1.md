# Math 132A Project 1

- Family Adventurer
  - 4 doors
- Classic Transporter
  - 2 doors

1. Let 

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

2. Now we will solve the problem using Excel:

   ![](imgs/excel.png)

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

3. Since the target campain cost $\$ 500000$, this means that we should take out $500000$​ in the target function. And since this campaign will raise the demand demand for the Classic Transporter next month by $20$ percent,  we have the new Linear Programming Problem:
    $$
    \begin{cases}
     		\text{Maximize  } \rightarrow z = 3700x_1 + 5300x_2 -500000\\
     		\text{Subject to:}\\
     		6x_1 +10.5x_2 \leq 48500\\
     		4x_1 + 2x_2 \leq 20000\\
     		x_2 \leq 4200\\
     		x_1 \geq 0, x_2 \geq 0
     \end{cases}
    $$
    We found that the optimal solution is when 
    $$
    \begin{cases}
     		x_1 = 3766\\ 
     		x_2 = 2467
     \end{cases}
    $$
    generating a profit of 
    $$
    3700 \times 3766 + 5300 \times 2467 = 26509300 \text{   dollars}
    $$
    But this is less than the original profit, which is $27009300$ dollars, so William Smith **should not undertake the campaign.**

4. Since William Smith can increase the plant capacity by $25$ percent, now he has $48500\times 1.25 = 60625 $ labor hours. Now we have the new linear programming problem:
    $$
    \begin{cases}
     		\text{Maximize  } \rightarrow z = 3700x_1 + 5300x_2\\
     		\text{Subject to:}\\
     		6x_1 +10.5x_2 \leq 60625\\
     		4x_1 + 2x_2 \leq 20000\\
     		x_2 \leq 3500\\
     		x_1 \geq 0, x_2 \geq 0
     \end{cases}
    $$
    We found that the optimal solution is when 
    $$
    \begin{cases}
     		x_1 = 3200\\ 
     		x_2 = 3500
     \end{cases}
    $$
    generating a profit of 
    $$
    3700 \times 3200 + 5300 \times 3500 = 30575000 \text{   dollars}
    $$
    Therefore, **William Smith should now produce $3200$ Family Adventurers and $3500$ Classic Transporters**.

5. Without the overtime, the company earns a profit of $27009300$ dollars. With overtime, the company now earns a profit of $30575000$ dollars. So the maximum amount of money William Smith would like to pay is
    $$
    32582900 - 30575000 = 2007900 \text{ dollars}
    $$

6. Both advertising and overtime pay.



