## Problem to Solve

Suppose you work at a store and a customer gives you $1.00 (100 cents) for candy that costs $0.50 (50 cents). You’ll need to pay them their “change,” the amount leftover after paying for the cost of the candy. When making change, odds are you want to minimize the number of coins you’re dispensing for each customer, lest you run out (or annoy the customer!). 

Implement a program in C that prints the minimum coins needed to make a given amount of change, in cents. 

*For the full background on Greedy Algorithms and detailed hints (like how to write your `calculate_quarters` function), read the official instructions here: [CS50 Cash Instructions](https://cs50.harvard.edu/x/psets/1/cash/)*

## Instructions

If you are unsure how to solve the problem itself, break it down into smaller problems that you can probably solve first. Here is the greedy algorithm you can use to solve this problem:

1. Prompt the user for change owed, in cents.
2. Calculate how many quarters you should give customer. Subtract the value of those quarters from cents.
3. Calculate how many dimes you should give customer. Subtract the value of those dimes from remaining cents.
4. Calculate how many nickels you should give customer. Subtract the value of those nickels from remaining cents.
5. Calculate how many pennies you should give customer. Subtract the value of those pennies from remaining cents.
6. Sum the number of quarters, dimes, nickels, and pennies used.
7. Print that sum.

## How to Begin

Open the terminal window at the bottom of your screen. You should find that your terminal prompt looks something like this:

```bash
student@codespace:/workspaces/codingrabbit-cs50-week1$
```

Next, execute the following command to change into the `cash` directory where you will write your program:

```bash
cd cash
```

Your terminal prompt should now update to show you are inside the new folder:

```bash
student@codespace:/workspaces/codingrabbit-cs50-week1/cash$
```

You can now execute the `code` command to create a new file and open it in the editor:

```bash
code cash.c
```

This will create a blank file called `cash.c` in which you can write your code. 

## How to Test

Recall that you can compile your program by running:

```bash
make cash
```

If it compiles successfully, run your program with:

```bash
./cash
```

If you see an error message or get stuck, remember to **click the Coding Rabbit icon** on the left sidebar to ask your AI Teaching Assistant for help!
