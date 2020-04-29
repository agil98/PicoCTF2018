# pipe
Points: 110

## Category
General Skills

## Question
>During your adventure, you will likely encounter a situation where you need to process data that you receive over the network rather than through a file. Can you find a way to save the output from this program and search for the flag? Connect with `2018shell.picoctf.com 37542`.

### Hint
>Remember the flag format is picoCTF{XXXX}
>Ever heard of a pipe? No not that kind of pipe... This [kind](http://www.linfo.org/pipes.html)

## Solution
We can use `nc 2018shell.picoctf.com 37542 | grep picoCTF` to pipe the output of the connection to grep and locate the flag

### Flag
`picoCTF{almost_like_mario_a6975cdb}`