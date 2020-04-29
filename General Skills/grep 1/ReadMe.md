# grep 1
Points: 75

## Category
General Skills

## Question
>Can you find the flag in [file](files/file)? This would be really obnoxious to look through by hand, see if you can find a faster way. You can also find the file in /problems/grep-1_4_0431431e36a950543a85426d0299343e on the shell server.

### Hint
>grep [tutorial](https://ryanstutorials.net/linuxtutorial/grep.php)

## Solution
We can open the file and just print out the flag using `cat file | grep picoCTF`

### Flag
`picoCTF{grep_and_you_will_find_d66382d8}`