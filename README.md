# IntelliDirb-TestData

## Test 1

The first test data set was generated by running a small sized wordlist (1,830 words) with recursion disabled, for 25 iterations. The following python command was used:

```
python testbench.py -w ../dsstorewordlist.txt -t ../targets.txt -o ../out/test2 -x ../IntelliDirb -i 25 --opts="-x txt,html,php --no_recurse"
```

## Test 2

The second test data set was generated by running a big sized wordlist (20,477 words) with recursion disabled, for 5 iterations. The following python command was used:

```
python testbench.py -w ../big.txt -t ../targets.txt -o ../out/test3 -x ../IntelliDirb -i 5 --opts="-x txt,html,php --no_recurse"
```

## Test 3

The third test data set was generated by running a small sized wordlist (1,830) with recursion enabled, for 1 iterations. Basic exclusions were used to limit excessive recursion. The following python command was used:

```
python testbench.py -w ../dsstorewordlist.txt -t ../targets.txt -o ../out/test1 -x ../IntelliDirb -i 1 --opts="-x txt,html,php --exclude vendor,cache,assets,styles,protected,media,images"
```