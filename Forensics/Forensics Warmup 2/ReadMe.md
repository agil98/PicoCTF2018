# Forensics Warmup 2
Points: 50

## Category
Forensics

## Question
>Hmm for some reason I can't open this [PNG] (files/flag.png)? Any ideas?

### Hint
>How do operating systems know what kind of file it is? (It's not just the ending!
>
>Make sure to submit the flag as picoCTF{XXXXX}

## Solution
Opening the file in a image viewer software will be able to open the file without any problems.

One can also use `file flag.png` to find the filetype. It will show that the image is actually a _jpg_.

### Flag
`picoCTF{extensions_are_a_lie}`