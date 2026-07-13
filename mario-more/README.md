## Problem to Solve

In a file called `mario.c` in a folder called `mario-more`, implement a program in C that recreates two adjacent pyramids of blocks using hashes (`#`), separated by a gap of two spaces. 

Your program should prompt the user for an `int` between 1 and 8, inclusive, for the pyramid's height. If the user inputs `4`, the pyramid should look exactly like this:

```
   #  #
  ##  ##
 ###  ###
####  ####
```

*For the full background on Super Mario Bros. and detailed hints on how to implement your loops, read the official instructions here: [CS50 Mario (More) Instructions](https://cs50.harvard.edu/x/psets/1/mario/more/)*

## Instructions

If you are unsure where to start, break the problem down into these smaller steps:

1. **Prompt for Height:** Use a `do while` loop and `get_int` to prompt the user for the pyramid's height. 
2. **Validate Input:** If the user inputs a number outside the range of 1 to 8 (inclusive), your program should re-prompt them again and again until they provide a valid number.
3. **Print the First Pyramid (Left):** Use a loop to print the rows. Inside that loop, you'll need logic to print the correct number of spaces and hashes (`#`) for the left-aligned pyramid.
4. **Print the Gap:** Print exactly two spaces (`  `) to separate the pyramids.
5. **Print the Second Pyramid (Right):** Print the correct number of hashes (`#`) for the right side. (Notice that the right pyramid does not need spaces printed *after* the hashes).
6. **Don't Forget the Newlines:** Make sure each row ends with a `\n` so the next row starts on a new line!

## How to Begin

Open the terminal window at the bottom of your screen. You should find that your terminal prompt looks something like this:

```bash
student@codespace:/workspaces/codingrabbit-cs50-week1$
```

Then execute the following command to change directories into that folder:

```bash
cd mario-more
```

Your terminal prompt should now update to show you are inside the new folder:

```bash
student@codespace:/workspaces/codingrabbit-cs50-week1/mario-more$
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
