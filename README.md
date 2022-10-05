# lab04-lsystems

I worked some with Megan Reddy

**Wheat Grammar Puzzle**
This the wheat L-System I generated in Houdini:

![](wheat_1.PNG) \
![](wheat_3.PNG) \
![](wheat_2.PNG) 

I used this grammar to generate this: \
Premise: F \
Rule 1: F=FF[-FF]F[-FF]FF-

Angle: 20


**Squares Grammar Puzzle**
This the squares L-System I generated in Houdini:

![](squares_1.PNG) \
![](squares_2.PNG) \
![](squares_3.PNG) 


I used this grammar to generate this: \
Premise: +F \
Rule 1: F=F+F-F-F+F

Angle: 90


**Custom Grammar Puzzle**
This the custom L-System I generated in Houdini:

![](custom_1.PNG) \
![](custom_3.PNG) \
![](custom_5.PNG) 


I wanted to start with something that looked like a flower at iteration
1, and morphed into a tree at later iterations. I think I have achieved this
goal. I roughly based the L-System on this: 

![](tree-no-leaves.jpg)
*Courtesy [All Things Nature](https://www.allthingsnature.org/what-are-deciduous-trees.htm)*

I used this grammar to generate this: \
Premise: FA \
Rule 1: A = !F[----^F\^^A-FB][++++&F&&-AFB]F[F\^^AFB][F&&AFB]F \
Rule 2: B = ^F--F&&&F

Angle: 5


\
\
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
