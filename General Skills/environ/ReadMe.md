# environ
Points: 150

## Category
General Skills

## Question
>Sometimes you have to configure environment variables before executing a program. Can you find the flag we've hidden in an environment variable on the shell server?

### Hint
>unix [env](https://www.tutorialspoint.com/unix/unix-environment.htm)

## Solution
We can use the command `printenv | grep picoCTF` to print all the environment variables and parse them to obtain the flag.
 ```
 $ printenv | grep picoCTF
 SECRET_FLAG=picoCTF{eNv1r0nM3nT_v4r14Bl3_fL4g_3758492}
```

### Flag
`picoCTF{eNv1r0nM3nT_v4r14Bl3_fL4g_3758492}`