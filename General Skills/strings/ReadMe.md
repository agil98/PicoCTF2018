# strings
Points: 100

## Category
General Skills

## Question
>Can you find the flag in this [file](files/strings) without actually running it? You can also find the file in /problems/strings_0_bf57524acf558aca2081eb97ece8e2ee on the shell server.


### Hint
>[strings](https://linux.die.net/man/1/strings)

## Solution
We are given a file with non-printable characters. The command `strings` allows us to print printable character sequences that are at least 4 characters long. By piping the result of strings, we can use grep to search for the string picoCTF as follow `strings strings | grep picoCTF`

### Flag
`picoCTF{5tRIng5_1T_dd38f284}`