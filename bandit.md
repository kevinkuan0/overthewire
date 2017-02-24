#Notes for the game: Bandit from overthewire

##Level 0
bandit0
cat readme


##Level 1
boJ9jbbUNNfktd78OOpsqOltutMc3MY1
```shell
cat <-
```

##Level 2  
CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9

##Level 4  
```shell
find inhere -type f -exec file '{}' \; | grep text
```

##Level 5  
koReBOKuIDDepwhWk7jZC0RTdopnAYKh
```shell
ls -alR | grep 1033 | grep "rw\-"
find ./ -size 1033c
find . -type f -exec file '{}' \; | grep text
```

##Level 6  
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
```shell
find ./ -user bandit7 -group bandit6 -size 33c # basic
find / -user bandit7 -group bandit6 -size 33c 2>&1 | grep -v denied | grep -v No  # parse error and output together
find / -user bandit7 -group bandit6 -size 33c 2>/dev/null # ignore error
```
see http://stackoverflow.com/questions/2342826/how-to-pipe-stderr-and-not-stdout

