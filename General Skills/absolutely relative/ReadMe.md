# asbolutely relative
Points: 250

## Category
General Skills

## Question
>In a filesystem, everything is relative ¯\_(ツ)_/¯. Can you find a way to get a flag from this [program](files/vuln)? You can find it in /problems/absolutely-relative_3_c1a43555f1585c98aab8d5d2c7f0f9cc on the shell server. [Source](files/absolutely-relative).

### Hint
>Do you have to run the program in the same directory? (⊙.☉)7
>Ever used a text editor? Check out the program 'nano'

## Solution
Reading the given source code, we can see that the binary searches for a file _permission.txt_ with the contants _yes_ in it. By running, `echo -n "yes" > permissions.txt` the permissions file is created with _yes_ in it.

### Flag
`picoCTF{3v3r1ng_1$_r3l3t1v3_a97be50e}`