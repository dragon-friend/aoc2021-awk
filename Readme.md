# AWK scripts for the 2021 advent of code

## Written in POSIX AWK 

Constraints: Every script must be short, hopefully written in just one line. I'll add them all to this file and then write one markdown file per day to document the code

### Day 1:

Exercise 1: `awk '{n+=($1>a)}{a=$1}END{print n-1}' input`

Exercise 2" `awk '{n+=(c>d)}{d=c}{c=$1+a+b}{b=a}{a=$1}END{print n-2}' input`
