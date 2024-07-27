<div class="Image" align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/1/1e/Bridges-answer.png" alt="Logo" width="180" height="150" border-radius="25%">
</div>
<h1 align="center">Hashiwokakero Solver</h1>

## About: 
The project is based on a popular puzzle, variously known as "Hashiwokakero", "Hashi" or "Bridges". The program combines logic, search methods and data structure functionality to navigate through the Hashiwokakero puzzle. 
Data structures like 2D Numpy Arrays and Stacks have been used to store and manage the island-bridge information. <br>

The algorithm begins with using logic assignment and elimination in a loop to read and study the input data in order to build all compulsory bridges. 
This drastically reduces the size and complexity of the map, reducing computation time and increasing efficiency. <br>

The program then proceeds to use forward propagation from the first appearing island to assign bridge values to this highly scaled-down version of the map, choosing the biggest between available neighbouring islands. 
If a choice does not lead to the solution, it will use back propagation to fix the mistake and reach the desired, solved state.

## Built With:
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) 
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white) 
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) 


## Principle:
### Logic Bridges:
Some islands, when surrounded by a specific number of neighbours, must share a certain number of bridges with each neighbour in order to satisfy the puzzle conditions.
For example, islands numbered 12 must have 4 neighbours and should share 3 bridges with each to reach a correct solution. 
Similarly, island 11s must have 2 bridges and 4 neighbours whereas island 10s must have 1 bridge with 4 neighbours. <br>

We can make several more programing decisions depending on the number of neighbours the remaining islands have. 
For example, if island 9 has 3 neighbours it must share 3 bridges with all three and islands 8 and 7 follow the same with 2 bridges and 1 bridge respectively.
Island 6 will have 3 bridges with each neighbour if there are 3 neighbours and islands 5 and 4 follow the same with 2 bridges and 1 bridge respectively. 

## Working: 
<div class="Image" align="center">
  <img src="https://github.com/aryaman-sakthi/Hashiwokakero/blob/main/assets/Example.png" alt="Logo" width="400" height="420" border-radius="25%">
</div>
<br>
Each number represents an "island", while the dots represent the empty space (water) between the islands. Numbers larger than 9 are indicated by 'a' (10), 'b' (11) or 'c' (12). <br><br>

The aim is to connect all the islands with a network of bridges, satisfying these rules:
  1. All bridges must run horizontally or vertically
  2. Bridges are not allowed to cross each other, or other islands
  3. There can be no more than three bridges connecting any pair of islands
  4. The total number of bridges connected to each island must be equal to the number on the island

For example, after reading the 10-line input above, your program might produce this output:
<div class="Image" align="center">
  <img src="https://github.com/aryaman-sakthi/Hashiwokakero/blob/main/assets/Example Solved.png" alt="Logo" width="400" height="420" border-radius="25%">
</div>

## Conclusion:
This project is a part of the COMP3411/9814 course curriculum and aims to enhance understanding and application of computational problem-solving techniques. This project not only reinforces theoretical knowledge but also prepares for real-world applications of AI and computational problem-solving. Currently, the program is able to successfully solve puzzles up to 30x30.
