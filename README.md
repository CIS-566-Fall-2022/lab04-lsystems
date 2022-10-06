# Puzzle 1 Solution:

Premise: F

Rules: (- and + set to 28 degrees)

F=FF[-FF]F[-FF]FF-(20)

# Puzzle 2 Solution:

Premise: -AF

Rules: (- and + set to 90 degrees)

F=-F-F+F+F-F+

A=+A

# Custom Grammar:

I wanted to create a cherry tree branch like this

![HTB1XMVHXYEF6uJjSZFOq6xUvVXaC](https://user-images.githubusercontent.com/25019996/194197590-f8f46480-3a3d-4497-a980-238d86de227d.jpg)
![X03189-e1600439471391](https://user-images.githubusercontent.com/25019996/194197592-1118b4bc-389a-49ce-aa67-46bbc83abfaa.jpg)

I haven't gotten to the flowers and leaves yet, but I plan to add them for fun later and I'll update this readme when I do :) Here are a few iterations of my current setup:

<img width="676" alt="Screen Shot 2022-10-05 at 10 01 28 PM" src="https://user-images.githubusercontent.com/25019996/194197764-337a0d9a-aa26-4114-9659-0f1446f4e2f8.png">
<img width="725" alt="Screen Shot 2022-10-05 at 10 01 34 PM" src="https://user-images.githubusercontent.com/25019996/194197776-f1bc8fb7-9534-4b04-a51f-d0d671211045.png">
<img width="708" alt="Screen Shot 2022-10-05 at 10 01 39 PM" src="https://user-images.githubusercontent.com/25019996/194197783-6ceba3e4-8309-4300-bcde-bb8f544bc3b7.png">
<img width="702" alt="Screen Shot 2022-10-05 at 10 01 44 PM" src="https://user-images.githubusercontent.com/25019996/194197793-8691eebf-e528-4252-a0a6-353196fe1d37.png">
<img width="642" alt="Screen Shot 2022-10-05 at 10 01 49 PM" src="https://user-images.githubusercontent.com/25019996/194197805-18d1d205-f6f1-47ff-bfeb-8e7978a36e67.png">
<img width="673" alt="Screen Shot 2022-10-05 at 10 01 56 PM" src="https://user-images.githubusercontent.com/25019996/194197817-435b7975-88f1-40a4-af0f-7b0a817aa903.png">
<img width="673" alt="Screen Shot 2022-10-05 at 10 01 56 PM" src="https://user-images.githubusercontent.com/25019996/194197817-435b7975-88f1-40a4-af0f-7b0a817aa903.png">

heres the beginnings of an attempt at flowers, super rough and kind of broken (later I'll make them not colliding, sometimes in the middle of branches, more organic looking, etc.), but we have proof of concept!

<img width="386" alt="image" src="https://user-images.githubusercontent.com/25019996/194201866-f55b60cf-0b2c-4903-afe6-c9ba59561a29.png">

Here is the grammar I defined to create it:

Premise: FAC

Rules:

A = !~(25)FS/(30)FDA (main branch structure with one center branch and alternating single and double branches)

B = !~(10)F(0.03) (singular "unit" that makes up branches, used in S and D)

S = !/(20)[!!^BBO~(10)PBOB] (single branch)

D = [!!!^(20)BBOBO~(15)BOBOB]/30[!&(40)BBOBBO~(20)PBOBOBOPBOBB] (double branch)

P = S : 0.4 (P included in double and single branches grow into single branches with probability 0.4)

C = GHGH (stems for flower cluster, flowers themselves not included) right now I just stuck one of these onto the end of the premise but later I plan to make them come off the double and single branches with some probability

G = ///^(30)[!IIIII] (short flower stem)

H = ///^(30)[IIIIIII] (long flower stem)

I = !!~(15)F(0.01) (singular "unit" that makes up flower stems)

O = T : 0.3 (O gets turned into flower but T with probability 0.3)

T = [+(30)&(30)/(30)~(30)F(0.006, 0.022)F(0.006, 0.03)F(0.002, 0.035)F(0.004, 0.05)F(0.004, 0.04)F(0.003, 0.015)F(0.001, 0.005)] (a flower bud shape)

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
