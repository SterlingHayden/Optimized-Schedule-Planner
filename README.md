# Optimized-Schedule-Planner
We developed an optimization model using Pyomo to improve the University of Arkansas Data Science schedule planner by determining the ideal courses to take and when to take them.
To achieve this, we created data arrays containing essential information, including:
- Required courses for graduation  
- Course availability by semester  
- Corequisite and prerequisite relationships  
- Course difficulty levels  
- Student’s desired graduation timeline  
- Semester hour limits  
- Options for taking specific semesters off

  
Using Pyomo, we defined the objective function and established constraints that are well-commented in the code.


### Key Insights from the Resulting Schedule:
- Semesters with 13-15 credit hours yield the most balanced and realistic schedules.  
- Higher credit hour limits lead to impractical schedules.  
- Lower credit hour limits disrupt the course sequence and may require summer semesters.  
- Early semesters follow a relatively fixed course order due to prerequisites.

###**The full code and PowerPoint offer the best way to explore this project in detail.**







