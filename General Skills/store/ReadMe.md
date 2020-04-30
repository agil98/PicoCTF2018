# store
Points: 400

## Category
General Skills

## Question
>We started a little [store](files/) can you buy the flag? [Source](files/source.c). Connect with `2018shell.picoctf.com 43581`.

### Hint
>Two's compliment can do some weird things when numbers get really big!

## Solution
This problem deals with a integer overblow. We can see in the source code that the total cost of fake flag is calculated by `total_cost = 1000*number_flags` and it is then deducted from the balance `account_balance = account_balance - total_cost`. We can take advantange of this by making the total cost a negative value, thus increasing our balance. The number of flags we can order is a signed integer so it will use Two's Complement representation, therefore if the given number is too big, it will be represented as a negative value. Purchasing around the max value for an int, `2,147,483,647`, fake flags, we can earn enough money to buy the real flag.

### Flag
`picoCTF{numb3r3_4r3nt_s4f3_6bd13a8c}`