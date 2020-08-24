
# CSCE 155E 
## Lab 2.0 Worksheet

Name(s) and Login(s):



1. Dennis Ritchie, the creator of the C programming language,
was born on September 9th, 1941.  If he were still alive, 
how old would he be today?  Find out by running the `birthday`
program on the appropriate inputs and enter your solution here.

         78 years, 49 weeks, 6 days old


2. Bjarne Stroustrup, the creator of the C++ programming
language, the object-oriented extension of C, was born on 
December 30th, 1950.  How old is he today?

           69 years, 33 weeks, 6 days old


3. Software testing often involves testing code with known
"bad" input in an attempt to break it (sometimes this is 
referred to as *fuzzing*).  Try breaking the `birthday_cli`
program by giving it "bad" input and observe the consequences.
Give at least two examples of potentially bad input and the 
results you observe.

        Dennis 1941 9 --> Error: Invalid number of command line inputs

        Den nis 1941 9 9 --> bash: Den: command not found


4. Complete all the size and range entries below.

* `char`
  size: 1 byte
  range: -128 to 127
* `short int`
  size: 2 bytes
  range: -32768 to 32767 (0 to 65535 for unsigned)
* `int`
  size: 4 bytes
  range: -2147483648 to 214783647 (0 to 4294967295 for unsigned)
* `long int`
  size: 8 bytes
  range: -9223372036854775808 to 9223372036854775807 (0 to 18446744073709551615 for unsigned)
* `float`
  size: 4 bytes
  range: 7 digits of accuracy
* `double`
  size: 8 bytes
  range: 15 digits of accuracy


5. Use your working currency conversion to determine 
the exchange amounts for the following inputs:

  a) $250.25
         
         67.67 British Pounds and 8648.64 Japanese JPY
  
  b) $1,000.52
         
         270.14 British Pounds and 34577.97 Japanese JPY

  c) $968,410.12
         
         261470.73 British Pounds and 33468253.75 Japanese JPY
  


6. Suppose that you had used only `int` types
in your conversion program.  Would you be able 
to use it to convert the US national debt 
(which as of 2020 was \$26,009,754,625,487)?
Why or why not?

          You would not be able to convert it because the debt is greater than the range that int is capable of using.


7. Mixed types

a) Run the `area` program with 3 and 4 as inputs.  
What value do you get?  Is this result correct?

         0.000000 square units - incorrect


b) Execute the program again with inputs 3 and 5.
Does the program give correct results?  Why not?

         0.00000 square units - incorrect, the program is wrong
         area is a double but it is computing with integers (1/2) which would compute to 0
         the computation should be (double) 1 / 2 OR 1.0 / 2.0

c) Fix the program by editing the `area.c` source 
code so that the program produces correct results.

         a) 6.000000 square units
         b) 7.500000 square units


