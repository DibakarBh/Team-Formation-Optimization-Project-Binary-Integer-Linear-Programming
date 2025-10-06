# Overview

This project develops a binary integer linear programming (BILP) model to form optimal student groups on the basis of performance metrics. The objective is maximize overall group success score. Each student is evaluated across three skill areas — Communication Skills, Problem-Solving, and Presentation Skills — each weighted equally (0.4, 0.4, 0.2 respectively).

The model is implemented using the lpSolve package, with automatically generated sample data representing student skill levels. The optimization ensures:

- Each group contains exactly three members.

- Each student is assigned to exactly one group.

- The solution maximizes the sum of group success scores under these constraints.

Visualization of group performance and solution verification are conducted using ggplot2.

# Findings

The linear programming solver successfully achieved an optimal solution, confirming feasibility under all constraints.

- Each of the 15 students was assigned to a group with balanced skill distribution.

- Group 5 achieved the highest total success score, while Group 2 recorded the lowest — reflecting natural variance in skill combinations.

- The optimization framework demonstrated that combining students with complementary strengths across communication, problem-solving, and presentation leads to the most effective team configurations.

- The model can easily be adapted for real-world scenarios by substituting sample data with actual student or employee skill assessments.
