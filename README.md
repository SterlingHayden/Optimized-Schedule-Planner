# Optimized-Schedule-Planner
We developed an optimization model using Pyomo to improve the University of Arkansas Data Science schedule planner by determining the ideal courses to take and when to take them.

To achieve this, we created data arrays containing essential information, including:
- **Required courses for graduation**  
- **Course availability by semester**  
- **Corequisite and prerequisite relationships**  
- **Course difficulty levels**  
- **Student’s desired graduation timeline**  
- **Semester hour limits**  
- **Options for taking specific semesters off**

Using Pyomo, we defined the objective function and established constraints, as follows:
Course value mathematical formulation:

$$f(\bf{X}, i) = \sum_{j=1}^b \sum_{k=1}^c \left[\bf{X}_{ijk}\left(j + \frac{1}{c - k + 2}\right)\right]$$

Objective function mathematical formulation:

$$\min_{\bf{X}, \bf{P}} \sum_{j=1}^b \sum_{k=1}^c \bf{P}_{jk}$$


### Key Insights from the Resulting Schedule:
- **Semesters with 13-15 credit hours yield the most balanced and realistic schedules.**  
- **Higher credit hour limits lead to impractical schedules.**  
- **Lower credit hour limits disrupt the course sequence and may require summer semesters.**  
- **Early semesters follow a relatively fixed course order due to prerequisites.**
