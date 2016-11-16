# TestCases: 
This is a rough description of test cases which I used while writing test cases.

```
pish : X
tegj : L
prok : V
glob : I
```

1. If rhs token count is 1 and rhs is not a valid roman numeral. 
Display message `invalid translation` and terminate.

2. If lhs token count is not 1. 
{Display message <invalid translation> and program terminates.}

3. If rhs or lhs is empty the input line will be ignored by message format parser.

4. If lhs has more than one tokens the input line will be ignored by message format parser.

```
glob glob Silver is 34 Credits
glob prok Gold is 57800 Credits
pish pish Iron is 3910 Credits
```

1. If rhs token count is not 1. 
{Display message <invalid translation> and program terminates.}

2. If rhs is not a valid floating point number. 
{Display message <invalid translation> and program terminates.}

3. If at lhs a token has been reached that doesn't belong to the transaltion map but still there are even more subsequent tokens i.e., there should be only one such token. 
{Display message <invalid translation> and program terminates.}

4. If roman number formed out of all the token found in transaltion map is not validated. 
{Display message <no idea>.}

5. Check for valid poitive and negative floating point numbers.

##
how much is pish tegj glob glob ?
##
1. If expression has a token that doesn't belong to the transaltion map.
{Display message <no idea> and the program continues with the next qeustion.}

2. If the roman number formed out of all these tokens doesn't validates. 
{Display warning <syntactically wrong>.}

##
how many Credits is glob prok Silver ?
how many Credits is glob prok Gold ?
how many Credits is glob prok Iron ?
##
1. If token from credits map is reached and yet expression has any more subsequent tokens.
{Display message <no idea>.}

2. If the roman number formed is invalidated.
{Display warning <syntactically wrong>.}

3. If a token is reached which doesn't belong to translation map.
{Display message <no idea>.}