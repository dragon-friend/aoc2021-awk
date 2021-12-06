# AWK scripts for the 2021 advent of code

## Written in POSIX AWK 

Constraints: Every script must be short, hopefully written in just one line. I'll add them all to this file and then write one markdown file per exercise to document the code

### Day 1:

Exercise 1: `awk '{n+=($1>a)}{a=$1}END{print n-1}' input`

Exercise 2: `awk '{n+=(c>d)}{d=c}{c=$1+a+b}{b=a}{a=$1}END{print n-2}' input`

### Day 2

Exercise 1: `awk {($1=="forward")?h+=$2:($1=="up")?d-=$2:d+=$2}END{print h*d}' input`

Exercise 2: `awk '{if($1=="forward"){h+=$2;d+=a*$2}else{($1=="up")?a-=$2:a+=$2}}END{print h*d}' input`

### Day 3

Exercise 1: `awk '{split($1,t,"");for(i in t)f[i]+=t[i]}END{for(i in f){(f[i]>NR/2)?g+=2^(length($1)-i):e+=2^(length($1)-i)}{print g*e}}' input`
