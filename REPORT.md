# How I Used AI to Build a 2048 Solver

I decided to use an AI assistant to help me create different algorithms for solving the 2048 game. Instead of writing
every line of code by myself, I asked the AI for ideas, code examples, and ways to improve my functions.

---

## Rule-Based Algorithm

**Prompt:**

```
Let's just talk about how WIN the game 2048 using just the rules ? What tips you know about that ??
How better to do moves ?? We are talking just about how to achive the max_tile - 2048.
```

**ChatGPT (o4-mini-high):**

```
🧠 GOAL:
Get the 2048 tile — by merging tiles intelligently and avoiding getting stuck.

✅ 𝗛𝗨𝗠𝗔𝗡-𝗙𝗥𝗜𝗘𝗡𝗗𝗟𝗬 𝗦𝗧𝗥𝗔𝗧𝗘𝗚𝗬 𝗥𝗨𝗟𝗘𝗦:

1. Pick a corner and never move the big tile from it
   Usually bottom-left or bottom-right.

Always “push” tiles toward that corner.

If your largest tile moves out of the corner, you’re in danger.
```

_just description of the rules..._

_To recap: in that message, the AI described the basic strategy to win 2048, and I decided to incorporate it into my
code._ **Here’s the message I wrote:**

```
okay, now our task is to make the function-solver based on that rules. 

That is my previos function that i use for random solver: 

(There was the function that i use for the eandom solver)

you need to study that, and use the main structure of that function to write the Rule-Based solver in the same styel
using the function play_2048(). But be based not on random but on the rules that you provide me in the previos message. 
```

**ChatGPT (o4-mini-high):**

_AI wrote the solver function so that it integrates correctly with my existing code and follows the rules we discussed
earlier_

---

## MINIMAX

In my quest to improve the 2048 solver using AI techniques, I initially attempted to use a basic **Minimax algorithm**.

_I initially asked ChatGPT to generate a Minimax algorithm for the 2048 solver, but the result was not satisfactory in
terms of performance and clarity._

**Prompt to ChatGPT 4.0 mini:**

```text
Please write a Minimax solver for 2048 that is simple, efficient, and well-commented.
```

**Outcome review:**

* The code had logical structure but suffered from low performance and inconsistent 2048 results.
* It was clear but did not meet my goals for speed or reliability.

**Prompt to Google AI Studio:**

```
The next method I want to try is the Minimax algorithm. 
This is the basic structure of that algorithm: (CODE)
but it's too complicated and doesn't give good results for me. 
I need to make the solution better. So please improve the code, but not make it too complicated. 
Just try to make it faster and give better results.
```

**Outcome review:**

However, the output from Google AI Studio resulted in a complex and difficult-to-understand code. Despite the
enhancements, the model did not achieve the desired result of consistently reaching the _2048 tile_, but the algorithm
did it better now.

After not achieving satisfactory results with **Google AI Studio**, I decided to try **ChatGPT 4.0 mini** once again,
hoping for a simpler and more effective solution. **The prompt given to ChatGPT 4.0 mini was:**

```
Please use the provided code to make it less complicated but still capable of achieving good results. Remove the comments and provide the final, simplified solution.****
```

**Outcome review:**

The output was much more straightforward. The Minimax algorithm was optimized in a more efficient manner.
The algorithm was simpler to understand, and the results were more consistent.

The Minimax algorithm with Alpha-Beta pruning provides a reasonable approach to solving the 2048 game.
However, the solution could still benefit.

---

## EXPECTIMAX

At first, I decided to try the **Monte Carlo** method for solving the 2048 game. However, I quickly realized that it was
too slow and I will spend a lot of time to run it minimum 30 times. I know that **Monte Carlo** is so efficient, but I
decided to tre the **Expectimax**.

I turned to **Google AI Studio** for advice on potential alternatives, hoping to find a method that could solve the game
faster and more efficiently.

**My Prompt to Google AI Studio:**

```
Advise me on an algorithm to solve the 2048 game faster than Monte Carlo.
```

_**Google AI Studio** suggested that **Expectimax** could be a good option for this problem. Expectimax is a popular
algorithm
in decision-making tasks where outcomes are uncertain and can help make better predictions about possible moves._

My process mirrored the **Minimax** solver’s development: first I asked **Google AI Studio** to draft the algorithm,
then I refined and corrected it using **ChatGPT o4-mini**, which gave me the final implementation.

---

## Conclusion

For this project, I used AI to implement three different 2048 solvers: Rule-Based, Minimax, and Expectimax. While these
algorithms aren’t the most efficient or highest-performing, they work reliably and produce respectable results. I also
wrote helper functions to collect statistics and visualize the outcomes, so I’m satisfied with what I’ve achieved.

 

