# OPTIMIZATION-MODEL

*COMPANY*: COOTECH IT SOLUTIONS

*Name*: SATENDRA VEER SINGH

*INTERN ID*:CT04DG3324

*DOMIAN*: DATA SCIENCE

*DURATION*: 4 WEEKS

*MENTOR*: NEELA SANTOSH






### Task Using Jupyter Notebook

This Jupyter Notebook presents a comprehensive optimization task focused on maximizing profit through efficient production planning for a furniture manufacturing scenario. The goal is to determine the optimal number of **tables** and **chairs** a company should produce, subject to resource limitations and market constraints. This type of problem falls under **Linear Programming (LP)** and is solved using the **PuLP** library in Python.

#### Problem Definition and Setup

The optimization problem is framed as a **profit maximization** task. The decision variables are the number of tables and chairs to produce, both defined as non-negative integers. The profit per unit is \$200 for tables and \$75 for chairs. These values serve as coefficients in the objective function.

The company operates with limited resources:

* **Wood:** 600 board feet available
* **Labor hours:** 120 available
* **Finishing hours:** 80 available

Each furniture item consumes different quantities of these resources. For example, a table requires 30 board feet of wood, 5 labor hours, and 3 finishing hours, while a chair uses less: 10 board feet, 2 labor hours, and 1 finishing hour.

Market-based constraints are also applied:

* At least **5 tables** must be produced
* A maximum of **50 chairs** can be produced

#### Objective and Constraints

The LP problem is then formulated by combining the profit function and the constraints into the `pulp.LpProblem()` object. Constraints ensure resource usage does not exceed availability and market conditions are respected.

#### Optimization and Solution

Once the model is solved using PuLP’s solver, the output provides:

* **Optimal production plan:** Number of tables and chairs
* **Maximum achievable profit**
* **Resource utilization:** Actual use versus available resources

#### Analysis and Insights

The notebook evaluates **which constraints are binding**—meaning fully utilized—and also calculates **resource slack**. This helps understand which resources are limiting production.

A **sensitivity analysis** or **shadow price analysis** is conducted to determine the value of increasing each resource by one unit. This is useful for management decision-making on resource investment.

#### Visualization

The solution includes multiple visualizations using **Matplotlib** and **Seaborn**:

* **Bar chart**: Resource utilization as a percentage
* **Pie chart**: Contribution of tables vs. chairs to total profit
* **Line graph**: “What-if” analysis showing how increased wood availability impacts profit

The "what-if" scenario is particularly valuable as it simulates varying wood resources (from 600 to 800 in steps of 20) to see how profit improves. This dynamic exploration informs whether acquiring more raw materials would be cost-effective.

#### Business Takeaways

1. The optimized production mix ensures the best use of limited resources while satisfying business goals.
2. The analysis highlights bottlenecks in resources.
3. Insights such as shadow prices provide a clear direction on which resource investments can yield the highest returns.


**OUTPUT**: TASK 4



