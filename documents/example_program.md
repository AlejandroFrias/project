```
Basic for loop:

PARSER START
(generate|make)? (for)? loop from $START to $END
PARSER END

CODE START: java
for(int i = ${1:$START}; i < ${2:$END}; i++) {
    $0
}
CODE END

CODE START: python
for x in xrange(${1:$START}, ${2:$END}):
    $0
CODE END
```
