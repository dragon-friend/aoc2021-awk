# AWK scripts for the 2021 advent of code

## Written in POSIX AWK 

Constraints: Every script must be short, hopefully written in just one line. I'll add them all to this file and then write one markdown file per day to document the code

### Day 1:

Exercise 1: `awk '{n+=($0>a)}{a=$0}END{print n-1}' input`
