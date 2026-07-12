## Problem to Solve

In a file called `mario.c` in a folder called `mario-less`, implement a program in C that recreates a right-aligned pyramid of blocks using hashes (`#`). 

Your program should prompt the user for an `int` for the pyramid's height. If the user inputs `4`, the pyramid should look exactly like this:

```
   #
  ##
 ###
####
```

*For the full background on Super Mario Bros. and detailed hints on how to implement your loops, read the official instructions here: [CS50 Mario (Less) Instructions](https://cs50.harvard.edu/x/psets/1/mario/less/)*

## Instructions

If you are unsure where to start, break the problem down into these smaller steps:

1. **Prompt for Height:** Use a `do while` loop and `get_int` to prompt the user for the pyramid's height. 
2. **Validate Input:** If the user inputs a number less than 1, your program should re-prompt them again and again until they provide a valid number.
3. **Print the Pyramid:** Use a loop to print the rows. Inside that loop, you'll likely need two more loops: one to print the correct number of spaces, and one to print the correct number of hashes (`#`) for that row.
4. **Don't Forget the Newlines:** Make sure each row ends with a `\n` so the next row starts on a new line!

## How to Begin

Open the terminal window at the bottom of your screen. You should find that your terminal prompt looks something like this:

```bash
student@codespace:/workspaces/codingrabbit-cs50-week1$
```

Next, execute the following command to make a folder called `mario-less` in your codespace:

```bash
mkdir mario-less
```

Then execute the following command to change directories into that folder:

```bash
cd mario-less
```

Your terminal prompt should now update to show you are inside the new folder:

```bash
student@codespace:/workspaces/codingrabbit-cs50-week1/mario-less$
```

You can now execute the `code` command to create a new file and open it in the editor:

```bash
code mario.c
```

## How to Test

Recall that you can compile your program by running:

```bash
make mario
```

If it compiles successfully, run your program with:

```bash
./mario
```

If you see an error message or get stuck, remember to **click the Coding Rabbit icon** on the left sidebar to ask your AI Teaching Assistant for help!
