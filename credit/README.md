## Problem to Solve

In a file called `credit.c` in a folder called `credit`, implement a program in C that checks the validity of a given credit card number using **Luhn’s Algorithm**. 

Your program should prompt the user for a credit card number (using `get_long`) and then report whether it is a valid American Express, MasterCard, or Visa card number by printing exactly `AMEX\n`, `MASTERCARD\n`, `VISA\n`, or `INVALID\n`.

*For the full background on credit card formats and a detailed walkthrough of Luhn's Algorithm, read the official instructions here: [CS50 Credit Instructions](https://cs50.harvard.edu/x/psets/1/credit/)*

## Instructions

If you are unsure where to start, break the problem down into these smaller steps:

1. **Prompt for Input:** Use `get_long` to prompt the user for a credit card number.
2. **Calculate Checksum (Luhn's Algorithm):** 
   - Multiply every other digit by 2, starting with the number’s second-to-last digit, and add those products’ digits together.
   - Add that sum to the sum of the digits that weren’t multiplied by 2.
   - If the total’s last digit is 0, the number is mathematically valid!
3. **Check for Card Length and Starting Digits:**
   - **American Express:** 15 digits, starts with 34 or 37
   - **MasterCard:** 16 digits, starts with 51, 52, 53, 54, or 55
   - **Visa:** 13 or 16 digits, starts with 4
4. **Print the Result:** Print `AMEX\n`, `MASTERCARD\n`, `VISA\n`, or `INVALID\n` (if the checksum fails or the length/starting digits don't match any card).

## How to Begin

Open the terminal window at the bottom of your screen. You should find that your terminal prompt looks something like this:

```bash
student@codespace:/workspaces/codingrabbit-cs50-week1$
```

Then execute the following command to change directories into that folder:

```bash
cd credit
```

Your terminal prompt should now update to show you are inside the new folder:

```bash
student@codespace:/workspaces/codingrabbit-cs50-week1/credit$
```

You can now execute the `code` command to create a new file and open it in the editor:

```bash
code credit.c
```

## How to Test

Recall that you can compile your program by running:

```bash
make credit
```

If it compiles successfully, run your program with:

```bash
./credit
```

If you see an error message or get stuck, remember to **click the Coding Rabbit icon** on the left sidebar to ask your AI Teaching Assistant for help!
