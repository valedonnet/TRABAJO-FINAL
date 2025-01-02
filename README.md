In this repository, you can explore implementations of a Genetic Algorithm, Simulated Annealing, and the Travelling Salesman Problem.

This project was developed as the Final Project for the Data Science and Machine Learning program at 4Geeks Academy.

If you have any questions, feel free to contact me at valedonnet@gmail.com.
Thank you for your interest!


## Traveling Salesman Problem (TSP)

A combinatorial optimization problem that consists of finding the shortest route to visit a list of cities and return to the city of origin.

### Applications

- Microchip manufacturing.
- Arranging school bus routes for children in a school district.
- Meal delivering.
- Scheduling service calls, etc.

---

### Problem

Imagine 4 cities A, B, C, D. All the possible tours are:

\[
\begin{array}{llll}
A \to B \to C \to D & B \to A \to D \to C & C \to A \to B \to D & D \to A \to B \to C \\
A \to B \to D \to C & B \to A \to C \to D & C \to A \to D \to B & D \to A \to C \to B \\
A \to C \to B \to D & B \to C \to A \to D & C \to B \to A \to D & D \to B \to A \to C \\
A \to C \to D \to B & B \to C \to D \to A & C \to B \to D \to A & D \to B \to C \to A \\
A \to D \to B \to C & B \to D \to A \to C & C \to D \to A \to B & D \to C \to A \to B \\
A \to D \to C \to B & B \to D \to C \to A & C \to D \to B \to A & D \to C \to B \to A \\
\end{array}
\]

The goal is to find the shortest path among all these possibilities.

---

## Genetic Algorithm for TSP

### Steps:

1. **Initialization**:
   - Generate an initial population of random paths.

2. **Evaluation**:
   - Use a fitness function to calculate the total distance of each path.

3. **Parent Selection**:
   - Select pairs of paths based on their fitness (shorter paths are more likely to be chosen).

4. **Crossover and Mutation**:
   - Combine paths to create new offspring and introduce random mutations to maintain diversity.

5. **Survivor Selection**:
   - Replace less fit paths with the new offspring.

6. **Termination**:
   - Stop the algorithm when a predefined condition is met (e.g., a set number of generations).

### Diagram

![Genetic Algorithm Process](step.png)

---

### Advantages of Genetic Algorithms

- Effective for complex optimization problems.
- Does not require gradient information.
- Can escape local minima.

### Limitations

- May not guarantee the optimal solution.
- Computationally expensive for large populations or many generations.


