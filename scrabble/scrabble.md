# e-mærket Code Challenge - Scrabble™

Create a program that can calculate the Scrabble™ score of a word or sentence.

### Description

The program must be callable from the command line, and print out the result to the command line as well.

```bash
> php scrabble.php "Elev hos e-mærket"
```

Should output

```bash
 The Scrabble score of "Elev hos e-mærket" is: 26 
```

In the table below, each letter (Bogstav) is listed with it's score (Score) and availability (Antal).

If the word/sentence given has too many occurrences of a letter, the program should give an error and exit.

```bash
> php scrabble.php "XXX"
```

Should output

```bash
 Illegal word! Cannot use "X" more than 1 times. 
```

### Letters & scores

| Bogstav | Score | Antal | Bogstav | Score | Antal | Bogstav | Score | Antal |
|:-------:|:-----:|:-----:|:-------:|:-----:|:-----:|:-------:|:-----:|:-----:|
|   A     |   1   |   7   |    K    |   3   |   4   |    U    |   3   |   3   |
|   B     |   3   |   4   |    L    |   2   |   5   |    V    |   3   |   3   |
|   C     |   8   |   2   |    M    |   3   |   3   |    X    |   8   |   1   |
|   D     |   2   |   5   |    N    |   1   |   6   |    Y    |   4   |   2   |
|   E     |   1   |   9   |    O    |   2   |   5   |    Z    |   4   |   1   |
|   F     |   3   |   3   |    P    |   4   |   2   |    Æ    |   4   |   2   |
|   G     |   3   |   3   |    Q    |   0   |   0   |    Ø    |   4   |   2   |
|   H     |   4   |   2   |    R    |   1   |   6   |    Å    |   4   |   2   |
|   I     |   3   |   4   |    S    |   2   |   5   |    -    |   0   |   2   |
|   J     |   4   |   2   |    T    |   2   |   5   |         |       |       |


### Bonus questions

You do not have to code these. Just explain how you would solve them :)

- Can you modify your solution that it takes input from the command line instead?

```bash
> php scrabble.php
  Enter word: Elev hos e-mærket
  
  The scrabble score of "Elev hos e-mærket" is 26
```

- Can you modify your solution so that it *does not* use a loop (`for`, `foreach` or `while`)?
