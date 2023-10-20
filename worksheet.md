
# Computer Science I 
## Lab 2.0 Worksheet

Name(s) and Login(s):



1. Dennis Ritchie, the creator of the C programming language,
was born on September 9th, 1941.  If he were still alive,
how old would he be today?  Find out by running the `birthday`
program on the appropriate inputs and enter your solution here.
ANSWER

Please Enter Your First Name (no spaces) followed by ENTER: DennisRitchie 
Enter the year in which you were born: 2003
Enter the month in which you were born (1-12): 9
Enter the day of the month in which you were born (1-31): 9
Today is 2023/10/20
Your birthday was 2003/09/09
Hello, DennisRitchie.  You are 20 years, 5 weeks, and 6 days old today



2. Bjarne Stroustrup, the creator of the C++ programming
language, the object-oriented extension of C, was born on
December 30th, 1950.  How old is he today?
ANSWER

Please Enter Your First Name (no spaces) followed by ENTER: BjarnStrousstrup
Enter the year in which you were born: 2008
Enter the month in which you were born (1-12): 12
Enter the day of the month in which you were born (1-31): 30
Today is 2023/10/20
Your birthday was 2008/12/30
Hello, BjarnStrousstrup.  You are 14 years, 41 weeks, and 6 days old today



3. Software testing often involves testing code with known
"bad" input in an attempt to break it (sometimes this is
referred to as *fuzzing*).  Try breaking the `birthday_cli`
program by giving it "bad" input and observe the consequences.
Give at least two examples of potentially bad input and the
results you observe.
ANSWER

1) PS E:\labwrk\CSCE155-C-Lab02> .\a.exe mashal 2000 18 788
Today is 2023/10/20
Your birthday was
Hello, mashal.  You are 20 years, 12 weeks, and 0 days old today.

2)PS E:\labwrk\CSCE155-C-Lab02> .\a.exe munazaa 2000 20 56
Today is 2023/10/20
Your birthday was
Hello, munazaa.  You are 22 years, 3 weeks, and 3 days old today.

4. Complete all the size and range entries below.

* `char`
  size: 1 byte
  range: -128 to 127
* `short int`
  size:2 bytes
  range:-32768 to 32767
* `int`
  size:4 bytes
  range:-2,147,483,648 to 2,147,483,647 (signed) or 0 to 4,294,967,295 (unsigned)
* `long int`
  size:4 or 8 bytes 
  range:-2,147,483,648 to 2,147,483,647 (signed) or 0 to 4,294,967,295 (unsigned) for 8 byte.
* `float`
  size:4 bytes
  range: 7 digits of accuracy
* `double`
  size:8 bytes
  range: 15 digits of accuracy


5. Use your working currency conversion to determine
the exchange amounts for the following inputs:

  a) $250.25
  ANSWER

PS E:\labwrk\CSCE155-C-Lab02> gcc .\dollar.c
PS E:\labwrk\CSCE155-C-Lab02> .\a.exe
Please input the total amount of US Dollars: 250
Fee (10%): $25.00
You get:
88.88 GBP
14360 JPY
  b) $1,000.52
  ANSWER

PS E:\labwrk\CSCE155-C-Lab02> gcc .\dollar.c
PS E:\labwrk\CSCE155-C-Lab02> .\a.exe
Please input the total amount of US Dollars: 1000.52
Fee (10%): $100.05
You get:
355.68 GBP
57472 JPY


  c) $968,410.12
ANSWER
PS E:\labwrk\CSCE155-C-Lab02> git add *
PS E:\labwrk\CSCE155-C-Lab02> gcc .\dollar.c
PS E:\labwrk\CSCE155-C-Lab02> . .\a.exe
Please input the total amount of US Dollars: 968,410.12
Fee (10%): $96.80
You get:
344.12 GBP
55604 JPY



6. Suppose that you had used only `int` types
in your conversion program.  Would you be able
to use it to convert the US national debt
(which as of 2020 was \$26,009,754,625,487)?
Why or why not?
ANSWER

No using only int type would not be sufficient fo convert the US national debt of $26,009,754,624,487.
The maximum value that can be stored in an int is 2,147,483,647,which is far less than the national debt.
Therefore the program would not be able to accurately represent or handle such a large number.




7. Mixed types

a) Run the `area` program with 3 and 4 as inputs.  
What value do you get?  Is this result correct?


b) Execute the program again with inputs 3 and 5.
Does the program give correct results?  Why not?


c) Fix the program by editing the `area.c` source
code so that the program produces correct results.
