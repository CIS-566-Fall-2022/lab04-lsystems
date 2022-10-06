# lab04-lsystems

## 1. Wheat grammar

Started with trying to create the tree in 1st iteration. Then replaced each branch with that tree.

Grammar:

Premise = A

Rules:

A = F-F[-F-F-F][--F-F-]

F = FF[-FF]F[-FF]FF

<img width="200" alt="square1" src="https://user-images.githubusercontent.com/90112787/194322209-324282dd-c691-46a4-8f67-ab525d4a8c9e.jpg">
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/90112787/194322287-55045511-71b7-4b28-aded-11e851d072f4.jpg">


## 2. Square grammar

Started with trying to create the pattern in 1st iteration. Then replaced each step with that pattern.

Grammar:

Premise = +F

Rules:

F = F+F-F-F+F

<img width="200" alt="square1" src="https://user-images.githubusercontent.com/90112787/194323290-1e4b9411-42e9-496b-8234-f4d670648751.jpg">
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/90112787/194323300-2dc478b7-e366-4901-b70b-be2999f97ebe.jpg">
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/90112787/194392249-3d01a26d-3278-43ec-b92d-d338da004c77.jpg">



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
