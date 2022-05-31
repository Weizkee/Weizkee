data types

quialifiers 
  unsigned
    double positive value, but lose negative values. goes from 0 to ~4 billion (no negatives)
  short, long, const

int
  whole numbers, no decimal points
  always take up 4 bytes (32 bits) of memory; values are limited to 32 bits worth of information
  ~2 billion to the positive; 2 billion to the negative

char
  variables that will store single character. 
  always take up 1 byte (8 bit) of memory; values are limited to 8 bits worth of information
  ASCII
  A, 65
  a, 97
  0, 48
  
float
  real numbers, have decimal points
  always take up 4 bytes (32 bits) of memory; values are limited to 32 bits worth of information
  precision issues due to limited number of digits

double
  same as float but double
  always take up 8 bytes (64 bits) of memory; values are limited to 64 bits worth of information
  more precision then float; extra 32 bits to work with

void
  type, not a data type
  cannot be set as a variable, cannot assign a value to void
  functions can have void return type (dont return a value)
  int main (void)
  take no argument 
  placeholder for "nothing", no return values no parameters0

bool
  Boolean value, holding 2 distinct values
  True/False
  
string
  words, collections of characters
  
structures (structs) and defined types (typedefs)

in C if you want to create a variable you have to do 2 things; specify data type and give name
you can declare more then 1 variable of the same data type with "," but you should only declare variables when you need them
  double doub, double, dloat; 

  int number; //declaration number as int
  number = 11; // assignment of number
  char character; // declaration character as char
  character = 'T'; // assignment of character, single quotes for single chaaracter (double quotes for multi characters, string type)
  int number = 11; // initialization - declaration and assignment in same line (instead of 2 lines like above
  float decimal = 11.7; // initialization
  
you only habe to declare your variable 1 time, weird things happen if you declare same variable multiple times

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Operators

Arithmetic Operators
add +
subtract -
multiply *
divide /
modulus %; //give remainder number

x = x * 5;
x *= 5;

increase x by 1
  x = x + 1
  x += 1
  x++ //x-- to decrease by 1
  
Boolean expressions
  comparing values
  evaluate one of two values - true or false
  used in conditionals and loops
    conditionals - deciding which path to take in a fork
    loop - deciding whether or not to continue the loop
  sometimes in Boolean expressions we use variables with type bool, but it's not required
  in C every nonzero value is equivalent to true, and zero is false.
  
  two main types of Boolean expressions
    logical operators
      && - both variables have to be true
      || - OR, if either variable to true
      ! - NOT, x (true), !x (false)
    relational operators 
      < - less than
      <= - less than or equal to
      > - greater than
      >= - greater than or equal to
      == - equality, checks if the 2 variables have the same value
      != - inequality, checks if the 2 variables have different value
        = is assignment 
        == is equality
        DO NOT CONFUSE = AND ==

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

conditionals
  forks in the road depending on values of variable or user input
  
  if (boolean-expression) 
  {
  }
  
  if true "if" codes between {} will be executed in order 
  if false codes between {} will not be exeuted
  
  if (boolean-expression) 
  {
  }
  else
  {
  }
  
  if true "if" codes between {} will be executed in order 
  if false "else" codes between {} will be exeuted in order

  you can nest else if to create chains (mutually exclusive):

  if (boolean-expression) 
  {
  }
  else if (boolean-expression1)
  {
  }
  else if (boolean-expression1)
  {
  }
  else
  {
  }
  
  you can create not-mutually exclusive if else
  
  if (boolean-expression) 
  {
  }
  if (boolean-expression1)
  {
  }
  if (boolean-expression1)
  {
  }
  else
  {
  }
  
  switch ()
    depending on the input switch () will have varying outputs specified
  
  int x = getint();         //if the user enters 1, case 1 will be output and break; or the following cases does not execute ("fall through")
  switch(x)
  {
    case 1:
        printf("One!\n");
        break;
    case 2:
        printf("Two!\n");
        break;
    case 3:
        printf("Three!\n");
        break;
    default:
        printf("Sorry!\n");
        break;
  }
  
   int x = getint();         //if the user enters 4, all code below case 4 will execute because there is no "break;" like the above
  switch(x)
  {
    case 5:
        printf("Five, ");
    case 4:
        printf("Four, ");
    case 3:
        printf("Three, ");
    case 2:
        printf("Two, ");
    case 1:
        printf("One, ");        
    default:
        printf("Blast off!\n");
  }
  
  Ternary Operator
  for simple cases when evaluate true or false, you can use  ?: 
  
  int x = (boolean expression) ? 5 : 6
    if true x will be 5
        before :
    if false x will be 6
        after :

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Loops
  allows program to execute lines of code repeatedly
    while, do-while, for
  
  forever
    while (true)
    {
    }
    this is an infinite loop; lines of code between {} will execute repeatedly until you break (break; statement) or kill the program
    
  repeat until
    while (boolean expression)
    {
    }
    if boolean expression is true, lines of code between {} will execute over and over until boolean expression is false
    
  do while
    do
    {
    }
    while (boolean expression)
    this loop will execute lines of code between {} once, then if boolean expression is true, it will go back and repeat code until boolean expression is false
    guarantees code to run at least 1 time
  
  for loop
    for (int i = 0; i < 10; i++)   //int i starts at 0; execute code between {} while i less than 10; increase i by 1 each run
    {
    }
    repeat code between {} a specific number of times (10 times in above example)
    for (start; expression; increment)
    {
    }

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

linux command line
  unix-based system
  ctrl + l
    clears command line screen
  ls
    list - read out of all files in directory
  cd
    go to home folder
  cd *name*
    change directory to name
  cd .. 
    go to containing folder
  pwd
    present working directory
  mkdir *name*
    makes new folder with name
  cp <source> <paste name>
    make a copy of source (file cannot do directory)
  cp -r <directory> <paste name>
    make a copy of source (directory) 
  rm <file name>
    prompts y/n before removing file
  rm -f <file name>
    skips y/n prompt (there is no undo)
  rm -r <directory>
    prompts y/n before removing entire directory
  rm -rf <directory>
    skips y/n prompt (there is no undo)
  mv <source> <new name>
    rename source file to new name
  chmoid
  
  rmdir
  
  sudo
  
  ln
  
  man
  
  clear
  
  touch
  
  diff
  
  telnet
  
  
  







































































