# grep examples
## grep -c

```
input: grep -c "asthma" ./technical/biomed/rr37.txt
output: 145

input: grep -c "hospitalization" ./technical/biomed/rr37.txt
output: 91

input: grep -c "subject" ./technical/biomed/rr37.txt
output: 30
```

The "-c" flag prints the number of lines that contain the input string rather than the lines themselves.

## grep -i

```
input: grep -i -c "asthma" ./technical/biomed/rr37.txt
output: 147

input: grep -i -c "hospitalization" ./technical/biomed/rr37.txt
output: 94

input: grep -c "subject" ./technical/biomed/rr37.txt
output: 33
```

The "-i" flag prints the lines that contain the input string, ignoring letter cases. When combined with -c, it is clear that using -i resulted in more line matches.

## grep -v

```
input: grep -v -c "asthma" ./technical/biomed/rr37.txt
output: 429

input: grep -v -c "hospitalization" ./technical/biomed/rr37.txt
output: 483

input: grep -v -c "subject" ./technical/biomed/rr37.txt
output: 544

input: grep -v -c "" ./technical/biomed/rr37.txt
output: 
```

The "-v" flag prints the lines that do not contain the input string. 
When combined with -c, we can see the amount of lines that contain the input subtracted from the total amount of lines.
