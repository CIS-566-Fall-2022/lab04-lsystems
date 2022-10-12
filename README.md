# lab04-lsystems
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

ANSWER #1:\
Premise: F\
Rule: F->FF[-FF]F[-FF]FF-\
Angle: 20 degrees



ANSWER #2:\
Premise: -F\
Rule: F->F-F+F+F-F\
Angle: 90 degrees\

n = 1\
<img width="354" alt="image" src="https://user-images.githubusercontent.com/65415823/195440010-1156fc32-8440-412d-b9b2-029eb9472b0e.png">

n = 2\
<img width="365" alt="image" src="https://user-images.githubusercontent.com/65415823/195439867-e6d6d1f2-c7de-40ef-a91e-9774726b35e4.png">

n = 3\
<img width="444" alt="image" src="https://user-images.githubusercontent.com/65415823/195439666-9f9b5e85-7fb4-4eed-b612-248cb1204c27.png">

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
