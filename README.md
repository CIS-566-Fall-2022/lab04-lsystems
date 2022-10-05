# Submission
Name: Megan Reddy

## Wheat Puzzle Solution

Premise: `F` \
Rule: `F = FF[-FF]F[-FF]FF-` \

Iteration: 1 \
![image](puzzle_two_1.png)

Iteration: 2 \
![image](puzzle_two_2.png)

Iteration: 3 \
![image](puzzle_two_3.png)

## Square Puzzle Solution

Premise: `+F` \
Rule: `F = F+F-F-F+F` \

Iteration: 1 \
![image](puzzle_one_1.png)

Iteration: 2 \
![image](puzzle_one_2.png)

Iteration: 3 \
![image](puzzle_one_3.png)

## Custom Plant: Oak Tree

![image](custom_lsystem.png)

Premise: `FFFFA` \
A: `" B //// B //// B` \
B: `[^FFF-!!FFA]!!!FFF` 

For my custom plant, I chose an oak tree. I used the 3D turtle symbols described in [Houdini's documentation](https://www.sidefx.com/docs/houdini/nodes/sop/lsystem.html#turtle-commands) to create it. For the premise, I started by making a long stem since oak trees have a large base. For the grammar, I used two rules - one that scales the branch length `"` and rolls the tree counter-clockwise `/` and another that sculpts each branch by scaling thickness `!`, pitching them up `^`, and stepping forward `F`. Oak trees tend to have longer branches and a thicker base than what I have here, which could be a good future step to take. 


# lab04-lsystems
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

## 2. Square grammar puzzle
How about this one?\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. You can take this as an opportunity to design a grammar for your homework assignment! Include images of your grammar's output.

## Submission
- Create a pull request against this repository
- In your readme, list your solutions to the puzzles, then your custom grammar and images of a few iterations of output
- Profit
