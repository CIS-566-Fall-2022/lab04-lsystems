# lab04-lsystems
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

Solution:
![Screenshot 2023-10-04 192106](https://github.com/RachelDLin/lab04-lsystems/assets/43388455/e13e559c-0611-4a55-8aee-6882c6b23fa0)

I noticed that the image from the first iteration is used recursively as a new "line segment" in the second iteration. I used this idea to write a recursive rule that has one stem with two branches coming off of it. I also noticed that in the second iteration, each repeated segment rotates off of the previous one. To account for this, I added a rotation at the end of the entire recursive rule.

## 2. Square grammar puzzle
How about this one?\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

Solution:
![Screenshot 2023-10-04 192134](https://github.com/RachelDLin/lab04-lsystems/assets/43388455/f7989855-6e05-4ec3-abb6-a00b7de29a26)

Similar to the previous puzzle, the pattern is plugged recursively into itself. I simply made a recursive rule for the L-system that goes straight, turns clockwise, goes straight, turns counter-clockwise, goes straight, turns counter-clockwise again, goes straight, turns clockwise, and goes straight.

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. You can take this as an opportunity to design a grammar for your homework assignment! Include images of your grammar's output.

Solution:
![Screenshot 2023-10-04 192322](https://github.com/RachelDLin/lab04-lsystems/assets/43388455/62ba604e-4595-4ff2-a1d3-ec29eddd2e81)

I used the idea of a recursive rule that was implemented in the previous two parts. I started out creating a fern-like shape by having a middle stem with branches going off of it symmetrically that gradually taper towards the top of the branch. I then added a few commands to pitch down and roll clockwise at certain points in the rule. This was to add some more dimension to the shape and get a spiral shape.
