[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=13175034&assignment_repo_type=AssignmentRepo)
# Theory vs. Practice

- List 3 reasons why asymptotic analysis may be misleading with respect to
  actual performance in practice.

  Run time analysis is a way to get a general idea of how long a program might run 
  depending on its size n.

  1- When running the code the algorithm could end up with its best case scenario running much faster
  than what you initially expect.

  2- Run time analysis focuses on how a general algorithm grows over time as its input increases, but dismisses 
  constant factors that depending on the algortihm could impact how long it takes to run, since we are comparing elements
  maybe the operation needed to compare slows down the overall implementaition.

  3- It could also depend on the hardware that is running the algortihm

- Suppose finding a particular element in a binary search tree with 1,000
  elements takes 5 seconds. Given what you know about the asymptotic complexity
  of search in a binary search tree, how long would you guess finding the same
  element in a search tree with 10,000 elements takes? Explain your reasoning.

  The time complexity of a binary tree is O log<sub>2</sub>(n) so a binary tree with 1000 elements 
  it should take log<sub>2</sub>(1000) 9.965 iterations, if 9.965 iterations is equal to 5 seconds then one iteration
  would take about 0.501756 (5/9.965) seconds. A tree with 10000 should take around (log<sub>2</sub>(10000)) 13.2877 iterations,
  so I would guess it would take around 6.667 seconds 

- You measure the time with 10,000 elements and it takes 100 seconds! List 3
  reasons why this could be the case, given that reasoning with the asymptotic
  complexity suggests a different time.

  1 - The initial run might have been the best case scenario for the binary search tree

  2 - The binary could be unbalanced leading to "heavier sides" that could take longer to search through.

  3- The computer could have been interrupted in its process by some other program that would take a higher priority.
